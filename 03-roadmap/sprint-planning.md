# ⏱️ Cronograma de Sprints (MVP) — EduPath

Este documento organiza o backlog do MVP em ciclos de desenvolvimento de 2 semanas (Sprints), garantindo entregas incrementais e testes constantes com usuários.

---

## 📅 Planejamento de Sprints e Esforço Estimado

Abaixo está o mapeamento cronológico focado na liberação dos módulos principais da plataforma:

| Sprint | Foco do Incremento | Histórias Envolvidas | Estimativa Total (Story Points) | Status |
| :--- | :--- | :--- | :--- | :--- |
| **Sprint 1** | Base de Cadastro & Perfis | `ED-1` a `ED-4` | 21 SP | 🔓 Concluído |
| **Sprint 2** | Criação de Trilhas & App Mobile | `ED-12`, `ED-13`, `ED-14`, `ED-15`, `ED-16`, `ED-17` | 24 SP | 🏃‍♂️ Em Andamento |
| **Sprint 3** | Progresso & Emissão de Certificados | `ED-18` a `ED-23` | 24 SP | ⏳ Backlog |
| **Sprint 4** | Dashboards, KPIs & Relatórios | `ED-24` a `ED-28` | 29 SP | ⏳ Backlog |

---

## 🎯 Detalhamento dos Objetivos por Sprint

### 🔒 Sprint 1: Fundação do Sistema (Concluída)
* **Meta da Sprint:** Permitir que novos usuários (alunos e gestores) se cadastrem de forma segura e acessem suas respectivas áreas logadas.
* **Resultados Mapeados:** Arquitetura de banco de dados estruturada, rotas de API protegidas com tokens JWT e telas de login funcionais no Front-End.

### 🏃‍♂️ Sprint 2: Criação de Trilhas e Experiência Mobile (Em Execução)
* **Meta da Sprint:** Garantir que o Coordenador Pedagógico consiga publicar um curso e estruturar os módulos enquanto o Aluno já consegue visualizar tudo responsivamente no smartphone.
* **Mitigação de Riscos:** Testar a usabilidade e o carregamento dos componentes em dispositivos de telas menores (Mobile-First).

### ⏳ Sprint 3: Gamificação, Progresso e Recompensa (Próxima)
* **Meta da Sprint:** Automatizar o reconhecimento do esforço do aluno através de indicadores visuais de progresso e geração instantânea de certificados seguros em PDF.
* **Dependências Técnicas:** Integração com serviços de renderização de PDF em segundo plano no servidor de aplicação.

### ⏳ Sprint 4: Dashboards Executivos e Canais de Comunicação
* **Meta da Sprint:** Munir os gestores de RH e professores com métricas analíticas profundas de ROI e engajamento da turma, além de abrir o canal de mensagens direto na plataforma.
* **Indicadores Críticos:** Tempo médio de estudo por módulo e taxa de retenção por trilha de aprendizado.
