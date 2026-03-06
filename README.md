# 🗣️ OuvidorIA — Assistente de Consultas da Ouvidoria
> Transformando a complexidade dos dados públicos em diálogos acessíveis através de Inteligência Artificial

O governo disponibiliza um volume enorme de dados sobre a ouvidoria, mas consultá-los
exige conhecimento técnico e paciência para entender as APIs. 

O objetivo é criar um agente de IA conversacional que permite a qualquer cidadão ou
gestor fazer perguntas em linguagem natural sobre os dados da ouvidoria e receber
respostas precisas, sem precisar entender de código ou estrutura de banco de dados.

## 🛠️ Tecnologias Utilizadas
* Frontend: Streamlit

* Backend: Python, FastAPI

* IA & NLP: LlamaIndex, Ollama (LLMs locais)

* Banco Vetorial: Qdrant

* Infraestrutura: Docker

## 🧠 Como Funciona

Utilizamos uma arquitetura de **Retrieval-Augmented Generation (RAG)**. O sistema extrai e processa dados governamentais (arquivos PDF, HTML via Web Scraping do Fala.BR), transforma-os em embeddings vetoriais no Qdrant e utiliza um LLM via Ollama para gerar respostas precisas com base apenas no contexto oficial recuperado.

## 🚀 Quick Start com Docker

A forma mais fácil de rodar a aplicação:

```bash
cd ouvidorIA
./start.sh
```

Acesse: http://localhost:8501

## 📦 Instalação Manual

Se preferir rodar sem Docker:

```bash
cd ouvidorIA
pip install -r requirements.txt
streamlit run main.py
```

**Nota:** Você precisará ter Ollama instalado localmente.

## 📚 Documentação Completa do Projeto
Para acessar a engenharia de requisitos, pipeline de dados, arquitetura e demais detalhes, visite a nossa documentação completa em: https://luciano-freitas-melo.github.io/ouvidorIA/

## 👨‍💻 Equipe

<table>
  <tr>
    <td align="center"><a href="https://github.com/marcusmartinss"><img style="border-radius:50%;" src="https://avatars.githubusercontent.com/u/89209017?v=4" width="100px;" alt=""/><br/><sub><b>Marcus Martins</b></sub></a></td>
    <td align="center"><a href="https://github.com/luciano-freitas-melo"><img style="border-radius:50%;" src="https://avatars.githubusercontent.com/u/88516249?v=4" width="100px;" alt=""/><br/><sub><b>Luciano Freitas</b></sub></a></td>
    <td align="center"><a href="https://github.com/NickGehjk"><img style="border-radius:50%;" src="https://avatars.githubusercontent.com/u/108106812?v=4" width="100px;" alt=""/><br/><sub><b>Nicolas Bomfim</b></sub></a></td>
    <td align="center"><a href="https://github.com/PauloGoncalvesLima"><img style="border-radius:50%;" src="https://avatars.githubusercontent.com/u/18203100?v=4" width="100px;" alt=""/><br/><sub><b>Paulo Gonçalves</b></sub></a></td>
  </tr>
</table>
