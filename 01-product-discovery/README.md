# 🎯 Product Discovery — EduPath

Esta pasta centraliza os artefactos estratégicos gerados durante a fase de **Product Discovery** do EduPath. O objetivo deste ciclo foi alinhar a visão de negócio às reais necessidades do mercado de EdTech corporativo.

---

## 🗺️ Visão Macro da Jornada do Utilizador

Para garantir que a engenharia entenda o fluxo de valor antes de olhar para o backlog, mapeamos a jornada principal do aluno (**Carlos**) ponta a ponta:

```mermaid
graph LR
    A[Primeiro Acesso] --> B(Aceite da LGPD)
    B --> C{Dashboard Ativa}
    C -->|Iniciar Trilha| D[Consumo de Conteúdo]
    C -->|Visualizar Perfil| E[Métricas de Progresso]
    D --> F[Disparo de Webhook / n8n]
    F --> G[Análise Preditiva da IA]
## 👥 Matriz Resumida de Personas

| Persona | Papel no Ecossistema | Principal Dor / Necessidade | Solução Core no MVP |
| :--- | :--- | :--- | :--- |
| **Ricardo** | Coordenador Pedagógico | Alto tempo gasto a criar e modularizar treinamentos locais. | Construtor modular de trilhas sequenciais rápidas. |
| **Ana** | Gestora de RH | Falta de dados em tempo real sobre o engajamento das turmas. | Dashboard analítica consolidada com filtros por setor. |
| **Carlos** | Aluno / Colaborador | Falta de tempo e dispersão durante o consumo de cursos longos. | Aplicativo Mobile-First com alertas inteligentes de IA. |

---

## 📑 Documentação Detalhada

Explore os arquivos individuais para entender a fundo as definições deste ciclo:
* [Product Vision & Proposta de Valor](./product-vision.md) — Pilares de negócio e alinhamento estratégico.
* [Elevator Pitch](./elevator-pitch.md) — Posicionamento de mercado e diferenciais competitivos.
* [Personas do Produto](./personas.md) — Mapeamento aprofundado dos perfis de utilizadores.
* [Jornada do Utilizador](./user-journey.md) — Detalhamento dos pontos de contacto e fricção na experiência.
