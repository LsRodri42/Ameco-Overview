<div align="center">

<img src="https://img.shields.io/badge/-%E2%9A%A1_AMECO-1A3A8C?style=for-the-badge&logoColor=F5C200&labelColor=1A3A8C&color=1A3A8C" height="40"/>

# ⚡ AMECO
### Sustentabilidade e Economia para Água e Energia

<p>
  <img src="https://img.shields.io/badge/Status-Em%20Desenvolvimento-F5C200?style=flat-square&labelColor=1A3A8C" />
  <img src="https://img.shields.io/badge/Plataforma-Android%20%7C%20iOS-4CAF50?style=flat-square&labelColor=1A3A8C" />
  <img src="https://img.shields.io/badge/Público-Usuários%20Brasileiros-1A3A8C?style=flat-square" />
</p>

<br/>

> **Ajudamos brasileiros a monitorar, entender e reduzir o consumo de água e energia —**  
> **transformando hábitos cotidianos em impacto real para o planeta e para o bolso.**

</div>

---

## 🌱 O que é o AMECO?

O **AMECO** é um aplicativo mobile focado em sustentabilidade doméstica para o mercado brasileiro. Por meio de registro de contas, metas personalizadas e inteligência artificial, o app oferece:

- 📊 **Análise de consumo** de água e energia ao longo do tempo  
- 🏆 **Score de sustentabilidade** (0–100) com conquistas e gamificação  
- 🤖 **Chat com IA** para dicas personalizadas de economia  
- 💰 **Impacto financeiro** calculado com base no salário mínimo vigente  
- 🌍 **Alinhamento com os ODS da ONU** — objetivos 6, 7, 12 e 13  
- 🌿 **Métricas de CO₂ evitado** e equivalência em árvores salvas  

---

## 🏗️ Arquitetura Geral

```
AMECO
├── 📱 Frontend          React Native + Expo + TypeScript
│   ├── auth             Login, Registro, Recuperação de senha
│   ├── Dashboard        Visão geral do consumo e score
│   ├── Energy           Registro e histórico de energia
│   ├── Water            Registro e histórico de água
│   ├── IA               Chat com assistente de sustentabilidade
│   └── user             Perfil, metas e conquistas
│
└── ⚙️  Backend           Node.js + Express + Firebase Admin
    ├── /auth            Autenticação JWT + Firebase Auth
    ├── /contas          CRUD de contas de água e energia
    ├── /sustentabilidade Score, metas, conquistas e resumo
    └── /chat            Integração com OpenAI (GPT-4o-mini)
```

---

## 🛠️ Stack Tecnológica

| Camada | Tecnologia |
|--------|-----------|
| **Mobile** | React Native + Expo SDK |
| **Linguagem** | TypeScript |
| **Backend** | Node.js + Express |
| **Banco de dados** | Firebase Firestore |
| **Autenticação** | Firebase Auth (Email + Google OAuth) |
| **IA** | OpenAI API — `gpt-4o-mini` |
| **Versionamento** | Git + GitHub |
| **Metodologia** | Scrum |

---

## 📐 Identidade Visual

<div align="center">

| Cor | Hex | Uso |
|-----|-----|-----|
| 🔵 Azul Escuro | `#1A3A8C` | Primária / Marca |
| 🟡 Amarelo | `#F5C200` | Destaque / CTA |
| 🟢 Verde | `#4CAF50` | Sustentabilidade |
| ⚪ Background | `#F4F6FB` | Fundo geral |

</div>

---

## 🎯 Roadmap

- [x] Autenticação com e-mail e Google  
- [x] Registro manual e por scan de contas  
- [x] Score de sustentabilidade (0–100)  
- [x] Chat com IA integrado  
- [x] Metas e conquistas (6 achievements)  
- [ ] Notificações e dicas inteligentes  
- [ ] Ranking de sustentabilidade  
- [ ] Integração com concessionárias reais  
- [ ] IA preditiva de consumo  
- [ ] Relatórios avançados exportáveis  

---

## 🌐 ODS Contemplados

<div align="center">

| ODS 6 | ODS 7 | ODS 12 | ODS 13 |
|-------|-------|--------|--------|
| 💧 Água potável e saneamento | ⚡ Energia limpa e acessível | ♻️ Consumo e produção responsáveis | 🌍 Ação contra a mudança climática |

</div>

---

## 📁 Repositórios

> Os repositórios de código são **privados** durante o desenvolvimento.  
> O projeto será disponibilizado progressivamente conforme as versões forem estabilizadas.

| Repositório | Descrição | Status |
|-------------|-----------|--------|
| `ameco-app` | Frontend mobile (React Native + Expo) | 🔒 Privado |
| `ameco-api` | Backend REST (Node.js + Express) | 🔒 Privado |

---

<div align="center">

**Feito com 💛 para um Brasil mais sustentável**

<img src="https://img.shields.io/badge/⚡_AMECO-Sustentabilidade%20%26%20Economia-1A3A8C?style=for-the-badge&labelColor=1A3A8C&color=4CAF50" />

</div>
