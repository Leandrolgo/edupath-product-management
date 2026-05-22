# 🗂️ Backlog do Produto (User Stories) — EduPath

Este documento contém o Product Backlog do MVP do EduPath, refinado e priorizado utilizando a metodologia **MoSCoW** e dimensionado em **Story Points (SP)** utilizando a sequência de Fibonacci. Os critérios de aceitação seguem o padrão de especificação behavior-driven (**Gherkin**).

---

### 🟢 ED-01: Autenticação de Utilizadores e Consentimento LGPD
* **Prioridade:** 🔴 Must Have (Crítico para o lançamento)
* **Esforço:** 5 Story Points
* **Persona Alvo:** Carlos (Colaborador/Aluno) & Ana (Gestora de RH)
* **Métrica de Impacto:** Segurança jurídica e Ativação de Usuários

**História de Utilizador:**
> **Como** utilizador da plataforma EduPath (Aluno ou Gestor),  
> **Quero** realizar a autenticação segura utilizando e-mail corporativo/senha e aceitar explicitamente as políticas de privacidade,  
> **Para que** eu possa acessar os meus dados de forma segura e em conformidade com as diretivas da LGPD/RGPD.

**Critérios de Aceite:**

* **Cenário 1: Autenticação com sucesso**
  * **Dado** que o utilizador está na página de login do EduPath;
  * **Quando** insere um e-mail válido e a senha correta cadastrada pela empresa;
  * **E** clica no botão "Entrar";
  * **Então** o sistema deve autenticar o utilizador e redirecioná-lo para a Dashboard correspondente ao seu perfil (Aluno ou Gestor).

* **Cenário 2: Primeiro acesso e aceite da LGPD**
  * **Dado** que é o primeiro login do colaborador Carlos na plataforma;
  * **Quando** ele realiza a autenticação com sucesso;
  * **Então** o sistema deve travar a tela e exibir o termo de consentimento de uso de dados (LGPD);
  * **E** o botão "Continuar" só deve ser habilitado após ele marcar a caixa de seleção de aceite.

---

### 🔵 ED-02: Criação de Trilhas de Aprendizagem Dinâmicas
* **Prioridade:** 🔴 Must Have (Core Business do Produto)
* **Esforço:** 8 Story Points
* **Persona Alvo:** Ricardo (Professor/Coordenador)
* **Métrica de Impacto:** Eficiência Operacional (Redução do tempo de criação de cursos)

**História de Utilizador:**
> **Como** coordenador pedagógico ou criador de conteúdos,  
> **Quero** criar trilhas de aprendizagem compostas por módulos sequenciais, vídeos e artigos,  
> **Para que** eu possa estruturar treinamentos corporativos de forma modular e ágil.

**Critérios de Aceite:**

* **Cenário 1: Criação de estrutura de curso vazia**
  * **Dado** que o professor Ricardo está autenticado com o perfil administrativo;
  * **Quando** acede à área "Criar Trilha" e insere um título, descrição e imagem de capa;
  * **Então** o sistema deve salvar o rascunho do curso e habilitar o botão de "Adicionar Módulos".

* **Cenário 2: Ordenação sequencial obrigatória**
  * **Dado** que o Ricardo adicionou três módulos à trilha;
  * **Quando** ele marca a opção "Sequência Obrigatória";
  * **Então** o sistema deve impedir que o aluno Carlos assista ao Módulo 2 sem ter completado 100% do Módulo 1.

---

### 🟡 ED-03: Dashboard Analítica de Performance Corporativa
* **Prioridade:** 🟡 Should Have (Diferencial de Negócio)
* **Esforço:** 8 Story Points
* **Persona Alvo:** Ana (Gestora de RH)
* **Métrica de Impacto:** Retenção de Clientes B2B e Engajamento de Turmas

**História de Utilizador:**
> **Como** gestora de RH de uma empresa parceira,  
> **Quero** visualizar uma dashboard consolidada com indicadores de progresso, taxas de conclusão e tempo médio de estudo dos colaboradores,  
> **Para que** eu possa metrificar o ROI do investimento em treinamento e intervir em setores com baixa adesão.

**Critérios de Aceite:**

* **Cenário 1: Filtro de dados por departamento**
  * **Dado** que a gestora Ana está na tela inicial de relatórios;
  * **Quando** seleciona o filtro por "Departamento: Operações";
  * **Então** os gráficos de pizza e barras devem recalcular instantaneamente para exibir apenas as métricas de conclusão dos colaboradores daquele setor.

* **Cenário 2: Exportação de relatório consolidado**
  * **Dado** que a Ana precisa enviar os dados para a diretoria;
  * **Quando** ela clica no botão "Exportar PDF";
  * **Então** o sistema deve gerar um arquivo estruturado contendo o resumo executivo dos indicadores selecionados na tela em menos de 5 segundos.
