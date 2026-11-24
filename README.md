# Programacao para web

- **Discente:** Sarah Oliveira Lucas Diógenes
- **Disciplina:** Programação para Web
- **Atividade:** Semana 01 — Criando a primeira API com Flask

## Objetivo do projeto

Desenvolver a estrutura inicial de uma API de chamados de suporte, utilizando Python e o framework Flask, com gerenciamento do ambiente virtual e das dependências por meio da ferramenta uv.

Nesta primeira etapa, foi implementada a rota GET /, responsável por retornar uma mensagem indicando o funcionamento da API.

## Tecnologias Utilizadas

- Python 3.13.7
- Flask 3.1.3
- uv
- Git e GitHub

## Estrutura do projeto

```text
programacao-para-web/
├── .gitignore
├── app.py
├── pyproject.toml
├── README.md
└── uv.lock
```

- `app.py`: código principal da aplicação Flask e definição das rotas da API.
- `pyproject.toml`: configurações do projeto e declaração das dependências.
- `uv.lock`: registro das versões das dependências, garantindo a reprodutibilidade do ambiente.
- `.gitignore`: definição dos arquivos e diretórios que não devem ser versionados.
- `README.md`: documentação do projeto e instruções de instalação e execução.

## Instrução de como instalar as dependências

Com o Python e o uv previamente instalados, acesse a pasta do projeto e execute:

```bash
uv sync --locked
```

## Instrução de como executar a aplicação

Para iniciar o servidor Flask, execute:

```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

## Acesso à API

Após iniciar a aplicação, acesse pelo navegador: http://localhost:5000/

No GitHub Codespaces, utilize o endereço disponibilizado pelo encaminhamento da porta 5000.

A requisição GET / deverá retornar:

- Status HTTP: 200 OK
- Content-Type: application/json

Corpo da resposta:

```json
{
  "mensagem": "API de chamados em funcionamento"
}
```

## Verificação do funcionamento

A resposta da API pode ser conferida pelo terminal utilizando:

```bash
curl -i http://localhost:5000/
```
