# Portfólio Pessoal

Projeto desenvolvido para prática de Git, GitHub e GitFlow.

## Tecnologias

- HTML
- CSS

## Objetivo

Criar um pequeno portfólio pessoal enquanto aplico o fluxo de desenvolvimento com GitFlow.

## Histórico de desenvolvimento

O projeto foi desenvolvido utilizando um fluxo baseado em GitFlow, mantendo as branches `main` e `develop` e separando o desenvolvimento em feature, release e hotfix.

### 1. Versão inicial

Foi criada a versão inicial do portfólio contendo a estrutura básica da página, apresentação pessoal e competências.

Principais commits:

- `e47f4c6` — `feat: versão inicial do portifólio`
- `33f8007` — `Add initial README with project details`

### 2. Desenvolvimento da feature de projetos

A partir da branch `develop`, foi criada uma feature destinada à implementação da seção de projetos.

Branch utilizada:

`feature/projetos`

O desenvolvimento foi dividido em dois commits distintos:

- `84966f8` — `feat: cria estrutura da seção de projetos`
- `0b7b9d4` — `feat: adiciona conteúdo aos projetos`

Após a conclusão, a feature foi integrada à `develop`:

- `6940931` — `merge: integra feature de projetos`

### 3. Preparação da release 1.0.0

Com a feature concluída, foi criada a branch:

`release/1.0.0`

Durante a preparação da versão foi adicionada a seção de contato:

- `364ef03` — `feat: adiciona seção de contato para release 1.0.0`

A release foi então integrada à `main`:

- `a93b65b` — `merge: publica release 1.0.0`

Nesse momento foi criada a tag:

`1.0.0`

A release também foi integrada novamente à `develop`:

- `f65e663` — `merge: integra release 1.0.0 em develop`

### 4. Hotfix após a release

Após a publicação da versão `1.0.0`, foi simulada a identificação de um erro em produção.

A partir da `main`, foi criada a branch:

`hotfix/corrige-titulo`

A correção foi registrada no commit:

- `c8d1678` — `fix: corrige nome inteiro do portfólio`

O hotfix foi integrado na `main`:

- `ad2d371` — `merge: aplica hotfix de título`

E depois à `develop`:

- `01347a7` — `merge: integra hotfix de título em develop`

## Resumo do GitFlow

```text
main
│
├────────────── release/1.0.0
│                     │
│                     ├── seção de contato
│                     │
│                     └── merge → main
│                            │
│                         tag 1.0.0
│
│
└── hotfix/corrige-titulo
          │
          ├── correção do título
          ├── merge → main
          └── merge → develop


develop
│
├── feature/projetos
│       ├── estrutura dos projetos
│       ├── conteúdo dos projetos
│       └── merge → develop
│
├── release/1.0.0 → merge → develop
│
└── hotfix/corrige-titulo → merge → develop

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