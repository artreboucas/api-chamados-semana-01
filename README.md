# API de chamados de suporte — Semana 01

**Estudante:** Arthur Rebouças do Carmo

## Objetivo

Criar a estrutura inicial de uma API de chamados de suporte utilizando Python, Flask e uv. Nesta primeira etapa, a API disponibiliza uma rota inicial para verificar seu funcionamento, sem cadastro de chamados ou banco de dados.

## Requisitos

- Python 3.10 ou superior
- uv ([instruções de instalação](https://docs.astral.sh/uv/getting-started/installation/))

## Instalação

No terminal, dentro da pasta do projeto, execute:

```bash
uv sync --locked
```

O uv criará o ambiente virtual e instalará as dependências registradas no arquivo `uv.lock`.

## Execução

Execute o comando abaixo, inclusive no GitHub Codespaces:

```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

## Teste da rota inicial

Acesse `http://localhost:5000/` pelo navegador. No Codespaces, abra a URL encaminhada da porta 5000 na aba **Ports** (Portas).

Também é possível testar a rota em outro terminal, mantendo o servidor em execução:

```bash
curl -i http://localhost:5000/
```

A requisição `GET /` deve retornar o status HTTP `200 OK`, o cabeçalho `Content-Type: application/json` e o seguinte objeto JSON:

```json
{
  "mensagem": "API de chamados em funcionamento"
}
```

Para encerrar o servidor, pressione `Ctrl+C` no terminal em que ele está sendo executado.
