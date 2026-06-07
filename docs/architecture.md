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

- interpretação educativa
- orientação de economia
- explicação de dados

Restrições:

- evitar previsões complexas sem base
- evitar respostas excessivamente técnicas
- priorizar clareza e utilidade prática

## Fluxo Geral

1. usuário acessa o app mobile
2. usuário informa dados ou consulta histórico
3. app processa parte da interface e chama APIs do backend
4. backend aplica regras, validações e integrações
5. dados são persistidos no Firebase
6. resultados retornam ao app

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
