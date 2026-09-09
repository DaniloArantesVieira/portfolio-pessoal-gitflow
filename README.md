# Portfólio Pessoal

Projeto desenvolvido para prática de Git, GitHub e GitFlow.

## Tecnologias

- HTML
- CSS

## Objetivo

Criar um pequeno portfólio pessoal enquanto aplico o fluxo de desenvolvimento com GitFlow.

## Evidências da atividade

As evidências do uso de Git, GitHub e GitFlow estão disponíveis na pasta:

`evidencias/`

Arquivos principais:

- `Gitflow.png` — histórico gráfico com feature, release e hotfix.
- `branch-tag-status.png` — branches principais, tag `1.0.0` e estado final do repositório.

## Fluxo utilizado

- `feature/projetos` criada a partir de `develop`
- feature integrada em `develop`
- `release/1.0.0` criada a partir de `develop`
- release integrada em `main` e `develop`
- tag `1.0.0` criada durante a release
- `hotfix/corrige-titulo` criado a partir de `main`
- hotfix integrado em `main` e `develop`