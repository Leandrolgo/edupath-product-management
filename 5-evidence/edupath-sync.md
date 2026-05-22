# 🔄 EduPath Sync — Arquitetura de Integrações & Automações

Este documento detalha a camada de mensageria, sincronização em tempo real e webhooks automatizados do EduPath. Essa estrutura foi projetada para permitir a orquestração de fluxos complexos em ferramentas como n8n e o disparo de gatilhos para Agentes de IA.

---

## 🗺️ Fluxo de Sincronização de Dados e Mensageria

> ⚠️ **Evidência de Arquitetura:** O diagrama abaixo mapeia como os eventos assíncronos trafegam do aplicativo mobile, passando pelo gateway da API, alimentando a fila de mensageria para consumo do ecossistema n8n e tomada de decisão dos Agentes de IA.

```mermaid
graph TD
    A[📱 Usuário / Aluno] -->|Conclui módulo no Mobile| B(🌐 API Gateway EduPath)
    B -->|1. Valida Sessão e JWT| C[(🗄️ Banco de Dados / Redis)]
    C -->|Estado Atualizado| D[🖥️ Painel Web do Gestor]
    B -->|2. Dispara Webhook Event: lesson.completed| E[⚙️ Orquestrador n8n]
    E -->|Se for o último módulo| F[🎓 Emissão de Certificado API]
    E -->|Gatilho de Dados| G[🤖 Agente de IA: Análise]
    G -->|Se houver ociosidade > 5 dias| H[💬 Alerta de Evasão via WhatsApp]

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#bbf,stroke:#333,stroke-width:2px
    style E fill:#f96,stroke:#333,stroke-width:2px
    style G fill:#6c6,stroke:#333,stroke-width:2px
    style H fill:#ff6,stroke:#333,stroke-width:2px
