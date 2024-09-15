# Ampliando o conhecimento de LLMs com dados externos

Este projeto utiliza Python para a criação de um sistema de Inteligência Artificial (IA) utilizando a arquitetura de Retrieval-Augmented Generation (RAG) com Large Language Models (LLMs).

## Pré-requisitos

- **Python**: 3.11.9 ou superior
- **Anaconda**: 3 2021.11 ou superior

## Estrutura de Pastas

A estrutura de pastas do projeto é organizada da seguinte forma:

```plaintext
.
├── documentos/
│   └── documento.pdf    # Documento PDF usado para criar a vector store
├── environment.yml      # Arquivo de configuração do ambiente Conda
├── oficina_rag.ipynb    # Notebook Python principal do projeto
└── README.md            # Documentação do projeto
```

## Dependências do projeto

### Configuração do Ambiente Conda

Para configurar o ambiente Conda, siga os passos abaixo:

1. **Clone o repositório**:

    ```bash
    git clone https://github.com/seu-usuario/seu-projeto.git
    cd seu-projeto
    ```

2. **Crie o ambiente Conda a partir do arquivo `environment.yml`**:

    ```bash
    conda env create -f environment.yml
    ```

3. **Ative o ambiente Conda**:

    ```bash
    conda activate oficina_rag
    ```

### Configuração da Key da OpenAI

Para executar o Notebook Python principal do projeto, que utiliza os serviços da OpenAI, você precisará de uma API key. Siga os passos abaixo para configurá-la:

1. **Crie uma chave de API da OpenAI**:

    - Acesse [OpenAI API](https://platform.openai.com/account/api-keys).
    - Faça login ou crie uma conta.
    - Gere uma nova chave de API.

2. **Configure a chave no projeto**:

    A chave pode ser configurada através de variáveis de ambiente. Adicione a linha abaixo ao seu arquivo `.env` na raiz do projeto:

    ```plaintext
    OPENAI_API_KEY=your_openai_api_key_here
    ```

    Alternativamente, você pode definir a variável de ambiente diretamente no terminal:

    ```bash
    export OPENAI_API_KEY=your_openai_api_key_here
    ```

## Como executar o projeto

Para executar o projeto, siga os passos abaixo:

1. **Ative o ambiente Conda**:

    ```bash
    conda activate oficina_rag
    ```

2. **Inicie o Jupyter Notebook**:

    Navegue até o diretório do projeto, inicie o Jupyter Notebook e execute o arquivo oficina_rag.ipynb:

    ```bash
    cd seu-projeto
    jupyter notebook
    ```

    Também é possível executar o notebook através do VSCode, selecionando o ambiente Conda criado anteriormente.