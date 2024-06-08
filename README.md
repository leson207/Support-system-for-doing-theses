# Support system for doing thesis
## Description:
A system that supports students doing their theses is designed as a chatbot.Aim at students in the information technology faculty of UET. Some of the main functions are:
- Searching for papers and theses
- Suggest teacher
- Suggest thesis's topic.
- Get teacher information.
- Answer questions about doing a thesis: qualification, start date, end date,...
## Commponent
- Crawler: Crawler for getting data.
- Data: Data use in the system. The full data can find at [Link](https://huggingface.co/datasets/VictorJuiz/thesis)
  - Teacher_UET: Teacher at the information technology faculty of UET
  - Paper_UET: Papers's of UET
  - Thesis_UET: Theses's of UET
  - Thesis_HUST: Theses's of HUST
  - Thesis_Foreign: Thesis of Stanford, Oxford, Toronto, Berkeley
  - Theis_Concate: Thesis_HUST + Thesis_Foreign
- Code:
  - System: Create system.
  - System_generate_test: Create a dataset to evaluate the generated answers for topic suggestions.
  - Embedding: Create a dataset to evaluate the embedding and reranking model.
## Evaluate
- Retrieval:
  - Consin similarity loss: 0.002/1
- Generate:
  - Context Relevant: 1/1
  - Answer Relevant: 0.6-0.9/1
  - Grounded: 1/1
## Example
Suggest thesis topic
![alt text](https://github.com/leson207/Support-system-for-doing-theses/blob/main/Report/Test_suggest_thesis.png?raw=true)
