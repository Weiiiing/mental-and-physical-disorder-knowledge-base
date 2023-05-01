# mental-and-physical-disorder-knowledge-base

A large-scale Chinese mental and physical disorder (MPD) knowledge graph combining multi-source data from the online medical consulting platform and domain lexicons.

## 1. Introduction
This project crawls through online medical consultation records of patients from websites and build an MPD knowledge ontology by extracting the core conceptual features of the text. Based on the ontology, an MPD knowledge graph containing 12,673 nodes and 82,195 relations is obtained using term matching with a domain thesaurus of each concept

## 2. File
- "01PA" is the node information of *patient*.
- "02MD" is the node information of *mental disorder*.
- "03MS" is the node information of *mental symptom*.
- "04MDR" is the node information of *mental drug*.
- "05PD" is the node information of *physical disorder*.
- "06PS" is the node information of *physical symptom*.
- "07PDR" is the node information of *physical drug*.
- "08BO" is the node information of *body*.
- "09SO" is the node information of *social cause or effect*.
- "10OP" is the node information of *operation*.
- "11PE" is the node information of *period* (last time).  
- "12PA_MD" is the relationship between *patient* and *mental disorder*.
- "13PA_MS" is the relationship between *patient* and *mental symptom*.
- "14PA_MDR" is the relationship between *patient* and *mental drug*.
- "15PA_PD" is the relationship between *patient* and *physical disorder*.
- "16PA_PS" is the relationship between *patient* and *physical symptom*.
- "17PA_PDR" is the relationship between *patient* and *physical drug*.
- "18PA_BO" is the relationship between *patient* and *body*.
- "19PA_SO" is the relationship between *patient* and *social cause or effect*.
- "20PA_OP" is the relationship between *patient* and *operation*.
- "21PA_PE" is the relationship between *patient* and *period*.

## 3. Corpus and Method
The dataset consists of patient’s consultation records from the online medical consultation platform named “The good doctor online”. This project included 102 hospitals and their URLs with psychosomatic departments in OMC platform. In order to expand the data size, we obtained the top five mental department URLs in 2021 and crawled through all the consultation records based on this merged list.

Domain lexicons were collected to perform term matching on the core concepts in the corpus, which in turn allows us to obtain information on the medical attributes of each patient, which is then organized to build a patient attribute knowledge graph (AKG).

- Disease thesaurus. This is derived from ICD-10 and DSM-5.

- Symptom knowledge base. This is derived from Chinese symptom knowledge base (CSKB), the terms in the symptom category (R) in ICD-10 and the Dalian University of Technology sentiment dictionary with negative class terms (“'boredom,” “abhorrence,” “sadness,” “fear,” “guilt,” “anger,” “panic,” “disappointment,” and “shame”).

- Drug knowledge base. This is derived from the Chinese medical knowledge graph (CMeKG) and the “A+ Medical Encyclopedia” website.

- Examination and surgical operation thesaurus. This is derived from CSKB and International Classification of Diseases Clinical Modification of 9th revision operations and procedures (ICD-9-CM3).

- Body thesaurus, i.e., human tissue terms. This is derived from the electronic medical record data of China Conference on Knowledge Graph and Semantic Computing (CCKS) 2018-2020, and the Sogo human anatomy thesaurus.

- Social element. This is derived from the class selection of the subject word list of the Modern Chinese Classification Dictionary (MCCD).

- Duration. This could be determined by the linguistic rule of “number + time unit”, where time units include “day,” “night,” “week,” “month,” “year”, such as “one week.”

## 4. Graph data structure
The MPD knowledge graph with 12,673 nodes and 82,195 relations was built. Taking a patient retrieval as example:

![patient](https://user-images.githubusercontent.com/55570101/235467772-9e2f4c76-b364-4ef8-b4e3-c059c32194ff.svg)

## Declaration
This work is the original research of the Text & Social Media Mining Lab (TSMM) of Yonsei university and the "Data Analysis and Computing" group in the School of Information Management of Nanjing University.
