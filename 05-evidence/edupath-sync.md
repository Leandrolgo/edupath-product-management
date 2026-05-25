# 📊 Evidências de Engenharia & Integrações — EduPath

Este diretório reúne as evidências arquiteturais e de integração do MVP do EduPath, demonstrando a viabilidade técnica do ecossistema e as conexões de microsserviços.

---

## 🛠️ Fluxo de Integração e Automação (n8n + IA)

```mermaid
graph TD
    A[Usuário: Consumo de Conteúdo] -->|Gera Evento| B[Banco de Dados PostgreSQL]
    B -->|Trigger de Mudança| C[Módulo Webhook do EduPath]
    C -->|Payload JSON via POST| D[Orquestrador n8n]
    D -->|Filtro & Higienização| E{Inatividade > 5 dias?}
    E -->|Sim| F[Agente de IA / LLM Contextual]
    E -->|Não| G[Apenas Atualiza Dashboard B2B]
    F -->|Gera Mensagem Customizada| H[API de Mensageria / WhatsApp]
    H -->|Notificação Push Ativa| I[Dispositivo do Colaborador]
