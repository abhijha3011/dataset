# dataset: corpus.7z
====================
All the open source data will be stored
Original source:
https://huggingface.co/datasets/samsum
======================================
Dataset Card for SAMSum Corpus
======================================

Dataset Summary as per the above link.

The SAMSum dataset contains about 16k messenger-like conversations with summaries.
 Conversations were created and written down by linguists fluent in English. 
 Linguists were asked to create conversations similar to those they write on a daily basis, reflecting the proportion of 
 topics of their real-life messenger convesations. The style and register are diversified - conversations 
 could be informal, semi-formal or formal, they may contain slang words, emoticons and typos. 
 Then, the conversations were annotated with summaries. 
 It was assumed that summaries should be a concise brief of what people talked about in the conversation in third person.
 The SAMSum dataset was prepared by Samsung R&D Institute Poland and is distributed for research purposes 
 (non-commercial licence: CC BY-NC-ND 4.0).

Languages:
English

Dataset Structure:
Data Instances:
The created dataset is made of 16369 conversations distributed uniformly into 4 groups based on the number of 
utterances in con- versations: 3-6, 7-12, 13-18 and 19-30. Each utterance contains the name of the speaker. 
Most conversations consist of dialogues between two interlocutors (about 75% of all conversations), 
the rest is between three or more people

The first instance in the training 
set: {'id': '13818513', 'summary': 'Amanda baked cookies and will bring Jerry some tomorrow.', 
        'dialogue': "Amanda: I baked cookies. Do you want some?\r\nJerry: Sure!\r\nAmanda: I'll bring you tomorrow :-)"}

Data Fields:
dialogue: text of dialogue.
summary: human written summary of the dialogue.
id: unique id of an example.

Data Splits:
train: 14732
val: 818
test: 819

Dataset Creation
Curation Rationale

In paper:
In the first approach, we reviewed datasets from the following categories: 
chatbot dialogues, SMS corpora, IRC/chat data, movie dialogues, tweets, comments data 
(conversations formed by replies to comments), transcription of meetings, written discussions,
 phone dialogues and daily communication data. Unfortunately, they all differed in some respect from the
  conversations that are typ- ically written in messenger apps, e.g. they were too technical (IRC data), 
  too long (comments data, transcription of meetings), lacked context (movie dialogues) or they were more of a 
  spoken type, such as a dialogue between a petrol station assis- tant and a client buying petrol. As a consequence, 
  we decided to create a chat dialogue dataset by constructing such conversa- tions that would epitomize the style of
 a messenger app.


Source Data
Initial Data Collection and Normalization
In paper:
We asked linguists to create conversations similar to those they write on a daily basis, 
reflecting the proportion of topics of their real-life messenger conversations. 
It includes chit-chats, gossiping about friends, arranging meetings, discussing politics, 
consulting university assignments with colleagues, etc. Therefore, this dataset does not contain any sensitive data or 
fragments of other corpora.


Who are the source language producers?
linguists

Annotations
Annotation process

In paper:
Each dialogue was created by one person. After collecting all of the conversations, we asked language experts 
to annotate them with summaries, assuming that they should (1) be rather short, 
(2) extract important pieces of information, (3) include names of interlocutors, 
(4) be written in the third person. Each dialogue contains only one ref- erence summary.


Who are the annotators?
language experts

Personal and Sensitive Information
None, see above: Initial Data Collection and Normalization
Considerations for Using the Data

Licensing Information
non-commercial licence: CC BY-NC-ND 4.0
