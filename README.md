# 🕸️ GraphRAG Tutorial — Neo4j + LLMs

<p align="center">
  <img src="./imgs/cover_page.gif" alt="alt text" width="700"/>
</p>

*A minimal end-to-end tutorial to build a knowledge-graph-powered RAG using Neo4j and OpenAI.*

![python](https://img.shields.io/badge/Python-v3.12.11-blueviolet)
![Neo4j](https://img.shields.io/badge/Neo4j-008CC1?logo=neo4j&logoColor=fff)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?logo=openai&logoColor=fff)
![LangChain](https://img.shields.io/badge/LangChain-0E8388?logo=python&logoColor=fff)
[![Anaconda](https://img.shields.io/badge/Anaconda-44A833?logo=anaconda&logoColor=fff)](#)
![GitHub last commit](https://img.shields.io/github/last-commit/DanielPuentee/neo4j-graphrag-tutorial)
[![GitHub Copilot](https://img.shields.io/badge/GitHub%20Copilot-000?logo=githubcopilot&logoColor=fff)](#)
![GitHub top language](https://img.shields.io/github/languages/top/DanielPuentee/neo4j-graphrag-tutorial)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

> Author: [Daniel Puente Viejo](https://www.linkedin.com/in/danielpuenteviejo/)

---

## 🎯 Objective

This repository shows how to **combine Neo4j + LLMs** to enable **reasoning-based retrieval** — going beyond vector similarity.  
We use a small **biomedical dataset** with drugs, diseases, biomarkers, and trials to compare **GraphRAG vs. classic RAG**.

---

## 🧠 Core Idea

Classical RAG retrieves text chunks by similarity.  
**GraphRAG** retrieves knowledge by relationships.

Example query:
> *“Which researchers in Spain studied immunotherapy drugs for breast cancer?”*

Classical RAG → unrelated text.  
GraphRAG → structured answer inferred from connected nodes.

---

## 🧩 Requirements
- Python used version: **3.12.11**
- Dependencies listed in `requirements.txt`
  ```python
  pip install -r requirements.txt
  ```
- `.env` file with the following variable:

  ```plaintext
  OPENAI_API_KEY=<your_api_key>
  NEO4J_URI=<your_neo4j_uri>
  NEO4J_USER=<your_neo4j_username>
  NEO4J_PASSWORD=<your_neo4j_password>
    ```



---

## 📃 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
