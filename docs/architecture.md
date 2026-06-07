# Arquitetura do AMECO

## Visão Geral

O ecossistema do AMECO está organizado em duas aplicações principais:

1. app mobile para interação com o usuário
2. backend para regras de negócio, integrações e apoio à IA

## Estrutura Atual

### App Mobile

Tecnologias:

- React Native
- Expo
- TypeScript

Responsabilidades:

- autenticação de usuário
- interface de consumo de energia
- interface de consumo de água
- histórico e gráficos
- interação com IA
- envio de dados ao backend

### Backend

Tecnologias:

- Node.js
- Express
- Firebase Admin

Responsabilidades:

- autenticação e validação
- persistência e leitura de dados
- regras de cálculo
- processamento de contas
- serviços de IA
- organização de rotas e controladores

## Módulo Central: Scanner de Contas com IA

O principal fluxo funcional do AMECO é o scanner de contas de água e energia.

Responsabilidades desse módulo:

- receber imagem capturada por câmera ou galeria
- enviar a imagem ao backend
- redimensionar e preparar a imagem para análise
- usar IA para extrair os dados relevantes da conta
- retornar os dados estruturados ao app
- permitir revisão antes de salvar
- evitar duplicidade de contas por usuário e mês de referência
- persistir os dados para histórico e cálculos posteriores

## Módulos Funcionais

### Energia

Entrada:

- potência
- quantidade de equipamentos
- horas de uso

Saída:

- consumo em kWh
- estimativa mensal
- valor estimado

### Água

Entrada:

- litros
- m3
- tarifa

Saída:

- consumo mensal
- estimativa de gastos
- histórico

### IA

Escopo atual:

- leitura de contas por imagem
- interpretação educativa
- orientação de economia
- explicação de dados

Restrições:

- evitar previsões complexas sem base
- evitar respostas excessivamente técnicas
- priorizar clareza e utilidade prática

## Fluxo Geral

1. usuário acessa o app mobile
2. usuário envia uma foto ou imagem da conta de água ou energia
3. app envia a imagem ao backend para análise
4. backend redimensiona a imagem e chama o serviço de IA
5. a IA extrai os dados principais da conta em formato estruturado
6. o app apresenta os dados para revisão do usuário
7. backend valida, evita duplicidade e persiste os dados no Firebase
8. o aplicativo usa essas informações para histórico, cálculos e estimativas

## Evolução Recomendada

### Curto Prazo

- padronizar contratos de API
- documentar entidades principais
- separar melhor serviços compartilhados

### Médio Prazo

- migrar backend para TypeScript
- introduzir camada de serviços mais formal
- criar documentação de endpoints

### Longo Prazo

- análises automáticas de histórico
- alertas personalizados
- integração com sensores e IoT
