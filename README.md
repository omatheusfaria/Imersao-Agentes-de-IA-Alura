# Imersão IA Alura + Google Gemini

Este repositório contém os projetos e códigos desenvolvidos durante a **Imersão de Inteligência Artificial da Alura em parceria com o Google**, focada na criação de agentes de IA utilizando o Google Gemini e o ecossistema LangChain.

## 🚀 Sobre a Imersão

A Imersão IA teve como objetivo construir, passo a passo, agentes de inteligência artificial capazes de realizar tarefas complexas. Ao longo de três aulas, exploramos desde a criação de um classificador inteligente até a orquestração de um agente autônomo com memória e capacidade de consulta a bases de conhecimento privadas.

## 📖 Conteúdo das Aulas

Cada aula representa um passo na evolução do nosso agente de IA.

| Aula | Título | Descrição | Link |
| --- | --- | --- | --- |
| 1 | **O Início da Jornada - Classificação Inteligente** | Introdução ao Gemini e LangChain. Criamos um agente classificador para um Service Desk, capaz de analisar uma solicitação e retornar uma saída estruturada (JSON) com a ação a ser tomada. | <a href="https://colab.research.google.com/github/omatheusfaria/Imersao-Agentes-de-IA-Alura/blob/main/Aula_01.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 2 | **Potencializando o Agente com RAG** | Implementamos a técnica de **Retrieval-Augmented Generation (RAG)**. O agente agora pode consultar uma base de conhecimento privada (documentos PDF) para responder a perguntas específicas sobre políticas internas, com citações das fontes. | <a href="https://colab.research.google.com/github/omatheusfaria/Imersao-Agentes-de-IA-Alura/blob/main/Aula_02.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| 3 | **Orquestrando o Agente com LangGraph** | Utilizamos o **LangGraph** para criar um agente multi-etapas e com estado. O agente agora segue um fluxo lógico: primeiro classifica a pergunta, depois decide se deve usar a base de conhecimento (RAG), pedir mais informações ou abrir um chamado. | <a href="https://colab.research.google.com/github/omatheusfaria/Imersao-Agentes-de-IA-Alura/blob/main/Aula_03.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |

## 🛠️ Tecnologias Utilizadas

- **Python**
- **Google Gemini API** (gemini-1.5-flash)
- **LangChain** (para estruturação e integração com o LLM)
- **LangGraph** (para orquestração de agentes)
- **FAISS** (para a criação do índice vetorial no RAG)
- **PyMuPDF** (para leitura de documentos PDF)
- **Jupyter Notebooks** (ambiente de desenvolvimento)

## ⚙️ Como Executar

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/seu-usuario/Imersao-Agentes-de-IA-Alura.git
    cd Imersao-Agentes-de-IA-Alura
    ```

2.  **Configure sua Chave de API:**
    - Os notebooks utilizam a `userdata` do Google Colab para buscar a chave da API do Gemini. Crie um segredo chamado `GEMINI_API_KEY` no seu ambiente Colab e adicione sua chave.
    - Como alternativa, você pode substituir `userdata.get('GEMINI_API_KEY')` diretamente pela sua chave no código.

3.  **Instale as dependências:**
    - Cada notebook possui no início os comandos `pip install` necessários para executar o código daquela aula.

4.  **Para as Aulas 02 e 03 (RAG):**
    - Você precisará fazer o upload dos arquivos PDF de políticas internas para o ambiente do Colab para que o sistema de RAG funcione corretamente.

## 👤 Autor

- **Matheus Faria**
- **LinkedIn:** www.linkedin.com/in/matheusfaria-dev
- **GitHub:** [[Matheus Faria]](https://github.com/omatheusfaria)

---
*Projeto desenvolvido com base no conteúdo da Imersão IA da Alura e Google.*
