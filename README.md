# mental-and-physical-disorder-knowledge-base

A large-scale Chinese mental and physical disorder (MPD) knowledge graph combining multi-source data from the online medical consulting platform and domain lexicons.

## 1. Introduction
- This project crawls through online medical consultation records of patients from websites and build an MPD knowledge ontology by extracting the core conceptual features of the text. Based on the ontology, an MPD knowledge graph containing 12,673 nodes and 82,195 relations is obtained using term matching with a domain thesaurus of each concept

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
