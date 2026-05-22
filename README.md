# EduPath 👥

> **Status do Projeto:** 🚀 MVP em Desenvolvimento / Planeamento de Integrações e IA  
> **Product Owner:** [Leandro Gasparello](https://linkedin.com/in/leandrogasparello)

## 📝 Descrição do Produto
Documentação oficial do produto EduPath — plataforma de aprendizagem personalizada para gestão de trilhas, acompanhamento de progresso e resultados de treinamentos para instituições de ensino e empresas.

---

## 🎯 1. Product Vision

### Elevator Pitch
Para instituições de ensino e empresas que perdem eficiência com treinamentos desorganizados e sem acompanhamento de resultados, o **EduPath** é uma plataforma web e mobile que centraliza a gestão de trilhas de aprendizagem, progresso dos alunos e indicadores de desempenho. Diferente de plataformas genéricas e complexas, o EduPath é simples, personalizável e focado em resultado.

### O Problema
* ❌ Trilhas de aprendizagem definidas sem critério pedagógico → baixo engajamento e retenção.
* ❌ Sem visibilidade do progresso dos alunos → gestores não identificam quem precisa de suporte.
* ❌ Comunicação fragmentada entre professor e aluno → retrabalho e desmotivação.
* ❌ Ausência de dados de desempenho → decisões sem base em resultados reais.

### Objetivos (OKRs)
* 📈 Elevar a taxa de conclusão de treinamentos em **40%** no 1º trimestre.
* ⏱️ **100%** dos alunos com progresso rastreado em tempo real.
* 📉 Reduzir em **70%** o tempo gasto em relatórios manuais.

---

## 👥 2. Personas & Jornadas

### Persona 1 — Professor Ricardo (Coordenador Pedagógico)
* **Frase:** *"Quero saber quem está aprendendo e quem está ficando para trás, sem precisar perguntar um por um."*
* **Frustração:** Gasta horas em relatórios manuais no Excel e tem comunicação dispersa.

### Persona 2 — Ana (Gestora de RH Corporativo)
* **Frase:** *"Preciso provar para a diretoria que os treinamentos geram resultado. Sem dados, não consigo."*
* **Frustração:** Dificuldade de engajar colaboradores e falta de relatórios automáticos de ROI.

### Persona 3 — Carlos (Aluno e Colaborador)
* **Frase:** *"Quero aprender no meu tempo, do meu jeito. Só me mostra o caminho."*
* **Frustração:** Plataformas difíceis de usar no celular e perda de progresso entre múltiplos dispositivos.

---

## 🗺️ 3. Roadmap de Produto (18 Meses)

| Fase | Período | Foco Principal | Entregáveis |
| :--- | :--- | :--- | :--- |
| **Fase 1: MVP** | 0 - 3 meses | Base & Operação | Cadastro, criação de trilhas, progresso em tempo real e certificados simples. |
| **Fase 2: V1.0** | 4 - 6 meses | Inteligência & Dados | Recomendação de trilhas com IA, dashboards de KPIs e alertas preditivos de evasão. |
| **Fase 3: V2.0** | 7 - 12 meses | Ecossistema & Integração | APIs públicas, integração com ERPs de RH e suporte automatizado. |
| **Fase 4: V3.0** | 13 - 18 meses | Engajamento Avançado | Gamificação (rankings/medalhas), relatórios em BI e Marketplace. |

---

## 🗂️ 4. Estrutura de Épicos e Backlog de Sprints

### 📌 Mapeamento de Épicos do Produto
*(Dica: Arrasta aqui a tua imagem do ecrã com a lista ED-1 a ED-6 que mostra os Épicos estruturados no teu ClickUp)*

### 📋 Sprints e Histórias em Execução

#### Sprint 2 — Trilhas e Aprendizagem (Em andamento)
* **Objetivo:** Entregar a criação, publicação e atribuição de trilhas de aprendizagem, além da experiência móvel inicial.
*(Dica: Arrasta aqui a imagem do ecrã da Sprint 2 com as Stories 20, 5, 6, 7, 8 e 21)*

#### Sprint 3 — Progresso e Certificados (Backlog)
* **Objetivo:** Entregar acompanhamento de progresso em tempo real e emissão automática de certificados.
*(Dica: Arrasta aqui a imagem do ecrã com as Stories 9, 10, 11, 12, 16 e 17)*

#### Sprint 4 — Dashboard, Relatórios e Comunicação (Backlog)
* **Objetivo:** Entregar dashboards pedagógicos/corporativos, relatórios exportáveis e canais de comunicação.
*(Dica: Arrasta aqui a imagem do ecrã da Sprint 4 com as Stories 13, 14, 15, 17 e 19)*

---

## ⚙️ 5. Processos do Time (DoR & DoD)

### Definition of Ready (DoR)
Para entrar na Sprint, a User Story precisa de:
1. Formato padrão executável (`Como... Quero... Para...`).
2. Critérios de aceite claros e testáveis.
3. Estimativa em Fibonacci feita pelo time.
4. Protótipo ou UI design anexado (Figma/Miro).

### Definition of Done (DoD)
Para ser considerada concluída, a User Story exige:
1. Código revisado (Peer Review) e integrado.
2. Homologação sem erros críticos pelo PO.
3. Documentação técnica atualizada no Confluence.

---

## 🔄 6. EduPath Sync — Arquitetura de Integrações & Automações

Para garantir a sincronização de dados entre múltiplos dispositivos (Plataforma Web e App Mobile) e permitir que empresas integrem o EduPath aos seus ecossistemas internos (ERPs de RH, Slack, WhatsApp), o produto conta com uma camada de mensageria e webhooks automatizados, ideal para orquestração via ferramentas de workflow (como n8n) e agentes de IA.

### 🗺️ Fluxo de Sindicância e Sincronização de Dados
