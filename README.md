# home-task-gen-ai

This GitHub repository contains two code files:

1) Home task for Data Scientist Deborah Lowi.ipynb
2) taskresults.json

The first ipynb file is a Jupyter notebook containing the Python code used in the project. The second file contains the results of the project in JSON format, i.e the AI responses to the list of pre-defined questions for both documents.

In order to run the code in the ipynb file, various packages will need to be installed if these are not already present. Details of required package installs are provided at the bottom of this README file. In addition, a ChatTogether API key will need to be used which can be set up here: https://api.together.ai/

# Project Limitations and Improvements

This was my first time working with LangChain, LangGraph and LLM models, which presented various challenges. However, it has been an interesting, challenging and rewarding project to complete and I am largely satisfied with the ouput results.

Some limitations and areas of improvement are listed below:

- **Model choie for embeddings, vector stores and llm choice** - for this project I used a HuggingFaceEmbeddings model, FAISS vector store and a ChatTogether llm, however limited time was spent researching the optimal model choice. To improve the project other models could be tried and results compared to find the optimal choice.

- **Document split method** - I used a RecursiveCharacterTextSplitter to split text, which was the recommended option based on a small amount of research, however I did not experiment with chunk size and overlap size. This could be tweaked in a future project to see if results are improved, or alternative text splitters could be explored.

- **Streamlit UI** - as there was limited time left to explore streamlit, I struggled to produce a meaningful and presentable UI using streamlit. Given more time, I would have liked to have improved this area of the project.


# Package Installs

```
pip install langchain
```
```
pip install langgraph
```
```
pip install streamlit
```
```
pip install langchain-community pypdf
```
```
%pip install -qU langchain-text-splitters
```
```
pip install -qU langchain-core
```
```
pip install langchain openai faiss-cpu
```
```
pip install sentence-transformers
```
```
%pip install --upgrade --quiet  langchain langchain-huggingface sentence_transformers
```
```
pip install pdfplumber
```
```
%pip install --upgrade langchain-together
```
