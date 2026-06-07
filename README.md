# AMECO Overview

Repositório de visão geral do projeto AMECO.

O AMECO é um aplicativo mobile voltado para sustentabilidade, economia financeira e monitoramento inteligente do consumo de energia elétrica e água. Este repositório centraliza a apresentação do projeto, sua arquitetura, sua organização e os passos iniciais para desenvolvimento.

## Objetivo

Este repositório existe para:

- apresentar o projeto de forma clara
- servir como ponto de entrada para novos colaboradores
- documentar a arquitetura geral
- organizar roadmap e próximos níveis da IA
- reunir links para os repositórios técnicos

## Estrutura do Ecossistema

Atualmente o projeto está dividido em dois repositórios principais:

- App Mobile: `Ameco-front-end-App-Mobile-`
- Backend: `Ameco-Back-End-Servidor`

## Stack Principal

### Frontend

- React Native
- Expo SDK 54
- TypeScript

### Backend

- Node.js
- Express.js
- JavaScript com migração recomendada para TypeScript

### Banco e Serviços

- Firebase Authentication
- Firebase Firestore
- Firebase Storage

## Funcionalidades Atuais

### Energia

- cálculo de consumo em kWh
- estimativa mensal
- estimativa de valor da conta

### Água

- cálculo de consumo mensal
- estimativa de gastos
- histórico de utilização

### Perfil e Conta

- cadastro
- login
- armazenamento de dados

### IA Educativa

Nível atual: `Nível 1 - IA Conversacional`

Funções atuais:

- explicar consumo
- responder dúvidas
- sugerir economia
- interpretar dados informados pelo usuário

## Documentação

- [Arquitetura](./docs/architecture.md)
- [Setup](./docs/setup.md)
- [Roadmap](./docs/roadmap.md)
- [Artigo Científico](./docs/publicacoes/artigo-cientifico-ameco.pdf)

## Distribuição do APK

O APK do AMECO não deve ficar versionado diretamente no histórico principal do repositório, porque é um arquivo binário grande e muda por versão.

Recomendação:

- manter o arquivo de APK apenas para preparo local
- publicar cada versão oficial em `GitHub Releases`
- adicionar no `README` do repositório o link da release mais recente
- página de releases: `https://github.com/LsRodri42/Ameco-Overview/releases`

Padrão sugerido de release:

- `v1.0.0`
- `v1.1.0`
- `v2.0.0`

## Direção Técnica

Prioridades atuais:

1. consolidar a base do app mobile
2. padronizar backend e contratos de API
3. manter IA com foco educativo e baixo custo operacional
4. evoluir documentação e organização do projeto

## Melhorias Recomendadas

- padronizar nomenclatura entre repositórios
- adicionar README nos repositórios mobile e backend
- migrar backend para TypeScript
- documentar endpoints e payloads
- definir estratégia de ambientes

## Missão

Ajudar pessoas a economizar água e energia por meio de tecnologia acessível, promovendo sustentabilidade, consciência ambiental e economia financeira.
