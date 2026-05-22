# 📋 User Stories & Critérios de Aceite — EduPath

Este documento contém o refinamento das Histórias de Utilizador que compõem o MVP e as primeiras versões do EduPath, mapeadas diretamente a partir do ClickUp.

---

## 🏃‍♂️ Sprint 2 — Trilhas e Aprendizagem

> **Objetivo da Sprint:** Entregar a criação, publicação e atribuição de trilhas de aprendizagem, além da experiência móvel inicial de navegação.

*(Arraste aqui a sua imagem `image_359c4c.png` para mostrar o board do ClickUp da Sprint 2)*

### ED-12 / Story 20 — Acessar plataforma pelo smartphone
* **Como** Aluno (Carlos)
* **Quero** aceder à plataforma EduPath diretamente através do navegador do meu smartphone
* **Para** conseguir estudar os conteúdos das minhas trilhas em qualquer lugar.
* **Critérios de Aceite:**
  * O layout deve ser 100% responsivo (Mobile-First).
  * O menu de navegação deve recolher para o formato "hambúrguer" em ecrãs menores que 768px.
  * O tempo de carregamento da página inicial no mobile não deve passar de 3 segundos em redes 4G.

### ED-13 / Story 5 — Criar trilha de aprendizagem
* **Como** Coordenador Pedagógico / Gestor (Ricardo / Ana)
* **Quero** criar uma nova trilha de aprendizagem definindo título e descrição
* **Para** estruturar um novo plano de capacitação na plataforma.
* **Critérios de Aceite:**
  * Deve haver um botão visível "Criar Nova Trilha".
  * Os campos "Título" (máx. 100 caracteres) e "Descrição" (máx. 500 caracteres) são obrigatórios.
  * O sistema deve salvar a trilha com o status inicial "Rascunho".

### ED-14 / Story 6 — Adicionar módulos à trilha
* **Como** Coordenador Pedagógico / Gestor (Ricardo / Ana)
* **Quero** adicionar e organizar múltiplos módulos ou aulas dentro de uma trilha
* **Para** sequenciar o conteúdo didático de forma lógica.
* **Critérios de Aceite:**
  * Deve permitir adicionar links de vídeos, textos ou PDFs em cada módulo.
  * Deve permitir reordenar os módulos através de arrastar e soltar (Drag and Drop).

### ED-15 / Story 7 — Vincular trilha aos usuários
* **Como** Coordenador Pedagógico / Gestor (Ricardo / Ana)
* **Quero** associar uma trilha de aprendizagem a alunos específicos ou setores da empresa
* **Para** direcionar o treinamento para o público correto.
* **Critérios de Aceite:**
  * Permitir a seleção de múltiplos utilizadores de uma lista.
  * Permitir vincular por "Tags" ou "Setor" (ex: Setor Comercial).

### ED-16 / Story 8 — Publicar trilha de aprendizagem
* **Como** Coordenador Pedagógico / Gestor (Ricardo / Ana)
* **Quero** mudar o status da trilha de "Rascunho" para "Publicada"
* **Para** que ela fique imediatamente disponível para os alunos vinculados.
* **Critérios de Aceite:**
  * Só permite publicar se a trilha tiver pelo menos 1 módulo com conteúdo.
  * Enviar uma notificação interna para todos os alunos vinculados após a publicação.

### ED-17 / Story 21 — Continuar progresso em múltiplos dispositivos
* **Como** Aluno (Carlos)
* **Quero** que o meu progresso de leitura e vídeos seja salvo centralizadamente
* **Para** retomar os estudos do ponto exato onde parei ao trocar de dispositivo.
* **Critérios de Aceite:**
  * O progresso do vídeo deve ser salvo a cada 5 segundos assistidos.
  * Ao carregar a aula, o sistema deve ler o estado do banco e posicionar o utilizador no segundo correto.

---

## 🗓️ Sprint 3 — Progresso e Certificados

> **Objetivo da Sprint:** Entregar o acompanhamento de progresso em tempo real para os gestores e a emissão automatizada de certificados para os alunos concludentes.

*(Arraste aqui a sua imagem `image_359c86.png` para mostrar o backlog da Sprint 3)*

* **ED-18 / Story 9:** Visualizar progresso individual (Visão do Aluno).
* **ED-19 / Story 10:** Monitorizar desempenho da turma (Visão do Professor).
* **ED-20 / Story 11:** Receber alertas de atraso (Automação de faltas).
* **ED-21 / Story 12:** Visualizar histórico de atividades do aluno.
* **ED-22 / Story 16:** Gerar certificado automático em PDF após conclusão de 100% da trilha.
* **ED-23 / Story 17:** Visualizar histórico de certificados emitidos no perfil.

---

## 🗓️ Sprint 4 — Dashboard, Relatórios e Comunicação

> **Objetivo da Sprint:** Fornecer dashboards executivos e pedagógicos consolidados, geração de relatórios exportáveis e canais de feedback entre tutores e alunos.

*(Arraste aqui a sua imagem `image_359caa.png` para mostrar o backlog da Sprint 4)*

* **ED-24 / Story 13:** Visualizar dashboard pedagógico com taxas de engajamento da turma.
* **ED-25 / Story 14:** Visualizar KPIs de treinamento (Tempo gasto, ROI, Notas).
* **ED-26 / Story 15:** Exportar relatórios consolidados em formatos CSV/Excel.
* **ED-27 / Story 18:** Receber notificações automáticas no sistema e e-mail.
* **ED-28 / Story 19:** Canal de comunicação direta (mensagens) entre professor e aluno.
