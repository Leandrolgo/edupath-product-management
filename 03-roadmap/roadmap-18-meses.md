# ⏳ Planeamento Estratégico Detalhado — 18 Meses

Este documento estabelece as dependências técnicas, marcos de entrega (milestones) e a distribuição de esforço ao longo do ciclo de vida planeado para o EduPath.

---

## 📅 Janela de Lançamentos e Dependências

A execução do roadmap do EduPath foi desenhada para mitigar riscos de engenharia, garantindo que a camada de infraestrutura esteja consolidada antes da entrada de funcionalidades complexas de IA.

```mermaid
gantt
    title Dependências Críticas de Engenharia
    dateFormat  YYYY-MM
    
    section Infraestrutura
    Setup de Segurança & LGPD    :done,   des1, 2026-04, 2026-06
    Módulos de Integração (n8n)  :active, des2, 2026-07, 2026-11
    
    section Funcionalidades
    App Mobile & Sincronia       :        des3, 2026-07, 2026-10
    Módulo de Agentes de IA      :        des4, 2026-11, 2027-03
