# Setup do Projeto

## Repositórios Atuais

O projeto está separado em dois repositórios:

- `Ameco-front-end-App-Mobile-`
- `Ameco-Back-End-Servidor`

## Pré-requisitos

- Node.js instalado
- npm instalado
- Expo CLI ou ambiente Expo funcional
- conta e credenciais Firebase configuradas

## App Mobile

Diretório:

`Ameco-front-end-App-Mobile-`

Comandos principais:

```bash
npm install
npm start
```

Atalhos disponíveis:

```bash
npm run android
npm run ios
npm run web
```

## Backend

Diretório:

`Ameco-Back-End-Servidor`

Comandos atuais:

```bash
npm install
node server.js
```

Observação:

O backend ainda precisa de padronização melhor de scripts em `package.json`, especialmente para desenvolvimento com recarga automática.

## Configuração Recomendada

### App Mobile

- definir arquivo de ambiente para URL da API
- padronizar acesso a serviços externos

### Backend

- validar variáveis em `.env`
- definir porta por variável de ambiente
- adicionar script `dev` com `nodemon`

## Próximos Ajustes Recomendados

- documentar variáveis de ambiente
- criar padrão de branches
- criar estratégia de versionamento
