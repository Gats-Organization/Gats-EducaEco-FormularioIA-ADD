# Projeto Flask: Aplicação de Previsão de Motivação em Sustentabilidade

Este projeto é uma aplicação web construída com Flask que utiliza um modelo de machine learning para prever a motivação dos usuários em relação à sustentabilidade. Os dados dos usuários são processados e enviados a uma API, sendo armazenados em um banco de dados MongoDB para posterior análise. O objetivo é facilitar a compreensão e o engajamento dos usuários em práticas sustentáveis, oferecendo insights personalizados.

## Sumário

- [Descrição do Projeto](#descrição-do-projeto)
- [Tecnologias Usadas](#tecnologias-usadas)
- [Instalação](#instalação)
- [Uso](#uso)
- [Arquivos Principais](#arquivos-principais)
- [Criador](#criador)

## Descrição do Projeto

Esta aplicação coleta dados de um formulário onde o usuário responde a perguntas sobre suas práticas sustentáveis, conhecimentos e preferências. Com base nessas informações, a IA classifica a motivação do usuário em diferentes categorias. O resultado é exibido na página web e também armazenado em uma API MongoDB para acompanhamento.

## Tecnologias Usadas

- **Python**: Linguagem de programação para desenvolvimento do backend e do modelo de machine learning.
- **Flask**: Framework web para criação da aplicação.
- **Pickle**: Biblioteca para serializar e desserializar o modelo de machine learning e o pré-processador.
- **Pandas**: Biblioteca para manipulação e transformação de dados do formulário.
- **Requests**: Utilizada para fazer requisições HTTP e enviar os dados do usuário à API.
- **Bootstrap**: Framework CSS para estilizar a interface web.
- **MongoDB**: Banco de dados usado para armazenar os resultados das previsões.

## Instalação

1. Clone o repositório:
    ```bash
    git clone https://github.com/seu-usuario/seu-repositorio.git
    cd seu-repositorio
    ```

2. Crie um ambiente virtual e ative-o:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # Para Linux/macOS
    venv\Scripts\activate  # Para Windows
    ```

3. Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```

4. Coloque os arquivos do modelo (`model.pkl`) e do pré-processador (`preprocessador.pkl`) no caminho especificado no código ou ajuste os caminhos conforme necessário.

5. Inicie o servidor Flask:
    ```bash
    python app.py
    ```

6. Acesse a aplicação no navegador em `http://127.0.0.1:5000`.

## Uso

1. Acesse o formulário inicial e preencha os campos requisitados, como nome, e-mail, faixa etária, renda familiar e outras questões relacionadas à sustentabilidade.
2. Clique em "Enviar" para que a aplicação processe suas respostas.
3. O resultado da previsão de motivação será exibido na tela.
4. Os dados também serão enviados e armazenados na API MongoDB configurada.

## Arquivos Principais

- **app.py**: Arquivo principal da aplicação Flask, que configura rotas, processa dados do formulário, faz a previsão e envia dados à API.
- **form.html**: Template HTML que exibe o formulário para os usuários responderem.
- **style.css**: Arquivo de estilo para a personalização visual da página.
- **model.pkl**: Arquivo serializado do modelo de machine learning.
- **preprocessador.pkl**: Arquivo serializado do pré-processador de dados.

## Criador
- Murilo de Oliveira Moreira