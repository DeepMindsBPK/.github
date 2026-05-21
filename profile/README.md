# MobIA — Gestão Inteligente de Leads

[![Microsoft Teams](https://img.shields.io/badge/Microsoft_Teams-6264A7?style=for-the-badge&logo=microsoft-teams&logoColor=white)](https://teams.microsoft.com)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)](https://azure.microsoft.com)

---

## 📋 Sobre o Projeto

**MobIA** é uma plataforma inteligente desenvolvida para o **Hackathon Prati** que revoluciona a forma como corretores gerenciam leads. Integrado a uma plataforma que simula o Microsoft Teams. O bot permite que vendedores registrem, acompanhem e organizem leads usando apenas **linguagem natural**, sem necessidade de acessar sistemas complexos manualmente.

Com dois bots especializados (CRM e Jira) e uma interface web intuitiva, a plataforma oferece uma experiência fluida tanto para **corretores** quanto para **gestores comerciais**.

---

## ✨ O Que Você Consegue Fazer

### 🏢 **Bot CRM — Gestão de Leads**
- Criar novos leads via chat natural
- Atualizar status e observações
- Agendar visitas automaticamente
- Consultar seus leads em tempo real
- Desambiguação inteligente de registros

### 📌 **Bot Jira — Acompanhamento de Tickets**
- Visualizar tickets abertos
- Adicionar comentários
- Atualizar status
- Receber notificações automáticas

### 🎯 **Interface Web**
- **Dashboard Corretor**: seus leads, metas e próximas visitas
- **Dashboard Gestor**: ranking, taxa de conversão, análises
- **Chat integrado** com os bots
- **Kanban visual** para organizar leads e tickets
- **Autenticação** com diferentes perfis de acesso

---

## 🎮 Como Funciona

**Fluxo do Corretor:**
```
1. Envia mensagem no Teams (ex: "Registre novo lead: João Silva, telefone 45 99999-0001")
2. Bot interpreta usando IA local
3. Extrai dados e atualiza CV CRM automaticamente
4. Confirma ação no chat
5. Lead aparece no dashboard/kanban
```

**Perfis de Acesso:**
- 👤 **Corretor**: Vê apenas seus leads e tickets
- 👨‍💼 **Gestor**: Acesso completo, pode reatribuir leads

---

## 🛠️ Stack Tecnológico

| Área | Tecnologia |
|------|-----------|
| **Backend** | Node.js, TypeScript, Bot Framework SDK |
| **Frontend** | HTML5, CSS3, JavaScript Vanilla |
| **IA** | LLM local (Qwen/LLaMA) |
| **Integrações** | Microsoft Teams, CV CRM API, Jira API |
| **Infraestrutura** | Oracle Cloud (Ubuntu 22.04), NGINX, SSL |
| **Deploy** | Netlify (Frontend), Azure Bot Service |

---

## 📁 Estrutura do Projeto

```
crm-bot/
├── 📄 README.md
├── 📄 package.json
│
├── 🎨 interface_front/          # Frontend - Chat + Kanban
│   ├── index.html
│   ├── app.js
│   └── style.css
│
├── 🔧 azure-bot/                # Bot CRM do Azure (Não implementado por falta de recurso)
│   ├── src/
│   │   ├── bot.ts
│   │   ├── api-client.ts
│   │   └── middleware/
│   └── package.json
│
├── 🔗 crm-jira-bot/             # Orquestração de bots
│   ├── api-crm/                 # Bot CRM
│   ├── api-jira/                # Bot Jira
│   ├── jira-mcp-server/         # MCP Jira
│   └── docker-compose.yml
│
└── 📚 docs/                     # Documentação
    ├── QUICK_START.md
    └── superpowers/
```

---

## 🧑‍💻 Time

| Nome | Função |
|------|--------|
| **Davi** | 🎯 Líder do Projeto |
| **Luiz** | 🤖 Bot Jira + Integração Teams |
| **Miguel** | ⚙️Infraestrutura |
| **Luan** | 🎨 Frontend, Infraestrutura |
| **Braian** | 💾 Backend, BD, API, VM Oracle |
| **Jhon** | 🔐 Pentest e Segurança |

---

## 🎯 Desafios do Hackathon

- **Desafio 3**: Bot no Teams para gestão de leads no CV CRM ✅
- **Desafio 5**: Bot no Teams para acompanhamento de tickets no Jira ✅

---

## 📚 Documentação

- [Quick Start](./docs/QUICK_START.md) — Guia rápido para começar
- [Navegação](./docs/NAVIGATION.md) — Guia de navegação da aplicação
- [Design e Arquitetura](./crm-jira-bot/docs/superpowers/specs/2026-05-21-bots-crm-jira-design.md)

---
## 📝 Licença

Este projeto foi desenvolvido para o **Hackathon Prati 2026** pela equipe **DeepMinds**.
