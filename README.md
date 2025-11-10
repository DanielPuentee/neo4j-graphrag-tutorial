# 🕸️ GraphRAG Tutorial — Neo4j + LLMs

![alt text](./imgs/cover_page.gif)   

*A minimal end-to-end tutorial to build a knowledge-graph-powered RAG using Neo4j and OpenAI.*

![python](https://img.shields.io/badge/Python-v3.10.15-blueviolet)
![Neo4j](https://img.shields.io/badge/Neo4j-008CC1?logo=neo4j&logoColor=fff)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?logo=openai&logoColor=fff)
![LangChain](https://img.shields.io/badge/LangChain-0E8388?logo=python&logoColor=fff)
[![Visual Studio Code](https://custom-icon-badges.demolab.com/badge/Visual%20Studio%20Code-0078d7.svg?logo=vsc&logoColor=white)](#)
[![Anaconda](https://img.shields.io/badge/Anaconda-44A833?logo=anaconda&logoColor=fff)](#)
![GitHub last commit](https://img.shields.io/github/last-commit/DanielPuentee/neo4j-graphrag-tutorial)
[![GitHub Copilot](https://img.shields.io/badge/GitHub%20Copilot-000?logo=githubcopilot&logoColor=fff)](#)
![GitHub top language](https://img.shields.io/github/languages/top/DanielPuentee/neo4j-graphrag-tutorial)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

> Author: [Daniel Puente Viejo](https://www.linkedin.com/in/danielpuenteviejo/)


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

## ⚙️ Workflow

1. **Create sample biomedical text files**  
2. **Generate `metadata.json` & `documents.csv`** with `create_text_chunks_csv.py`  
3. **Ingest into Neo4j** and build nodes/relationships  
4. **Ask multi-hop questions** through Cypher queries  
5. **Compare results vs. classical RAG**