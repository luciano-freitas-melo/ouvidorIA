---
hide:
  - navigation
  - toc
---

# OuvidorIA 

Bem-vindo ao repositório do **OuvidorIA**, um assistente virtual inteligente projetado para simplificar e fortalecer a comunicação entre o cidadão e as ouvidorias públicas no Brasil.

> 🚀 **Status:** Em desenvolvimento (Fase MVP) | **Stack:** RAG, LLMs, FastAPI, Streamlit

## 🎯 O Problema
Muitas vezes, o processo de registrar uma manifestação (como uma denúncia ou reclamação) pode ser complexo e burocrático. A linguagem técnica dos manuais e a dificuldade em formular um texto claro podem desestimular a participação cidadã de uma ferramenta essencial para a melhoria dos serviços públicos.

## ✨ Nossa Solução
O OuvidorIA surge como uma solução para este desafio. Utilizando **Inteligência Artificial e Processamento de Linguagem Natural**, nossa plataforma atua como uma ponte. Ela oferece ao cidadão uma interface conversacional simples para tirar dúvidas e organizar suas ideias, ao mesmo tempo que estrutura essas informações para facilitar a triagem pela gestão pública.

### 🧠 Como Funciona (Arquitetura RAG)
Nossa solução é construída com uma abordagem *Retrieval-Augmented Generation (RAG)*, garantindo que as respostas da IA sejam fundamentadas em documentos oficiais (como o portal Fala.BR e cartilhas governamentais), evitando alucinações.

* **Frontend:** Interface conversacional intuitiva construída com `Streamlit`.
* **Backend:** Orquestração de APIs utilizando `FastAPI`.
* **Motor de IA & RAG:** Integração com LLMs via `Ollama` e orquestração de contexto com `LlamaIndex`.
* **Banco Vetorial:** Armazenamento e busca semântica de documentos processados utilizando `Qdrant`.
* **Pipeline de Dados (ETL):** Web scraping inteligente com hash (MD5) e chunking de documentos para vetorização.

![Diagrama de Arquitetura do MVP](images/arquitetura-mvp.png){width="60%" style="display: block; margin: 0 auto"} 

## 👨‍💻 A Equipe

<table>
  <tr>
    <td align="center"><a href="https://github.com/marcusmartinss"><img style="border-radius:50%;" src="https://avatars.githubusercontent.com/u/89209017?v=4" width="100px;" alt=""/><br/><sub><b>Marcus Martins</b></sub></a></td>
    <td align="center"><a href="https://github.com/luciano-freitas-melo"><img style="border-radius:50%;" src="https://avatars.githubusercontent.com/u/88516249?v=4" width="100px;" alt=""/><br/><sub><b>Luciano Freitas</b></sub></a></td>
    <td align="center"><a href="https://github.com/NickGehjk"><img style="border-radius:50%;" src="https://avatars.githubusercontent.com/u/108106812?v=4" width="100px;" alt=""/><br/><sub><b>Nicolas Bomfim</b></sub></a></td>
    <td align="center"><a href="https://github.com/PauloGoncalvesLima"><img style="border-radius:50%;" src="https://avatars.githubusercontent.com/u/18203100?v=4" width="100px;" alt=""/><br/><sub><b>Paulo Gonçalves</b></sub></a></td>
  </tr>
</table>