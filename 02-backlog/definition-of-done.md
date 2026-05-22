# 🏁 Definition of Done (DoD) — EduPath

O **Definition of Done (DoD)** é o acordo de qualidade firmado entre o Product Owner e a equipa de Engenharia de Software. Uma História de Utilizador (User Story) ou Incremento de Sprint só será considerada "Concluída" (Done) e contabilizada na Velocity se cumprir 100% dos critérios abaixo.

---

## 🚀 Critérios Gerais de Conclusão (Checklist)

### 1. Qualidade de Código & Engenharia
- [ ] **Code Review:** O código foi revisto por pelo menos um Engenheiro Sénior e aprovado via Pull Request (PR).
- [ ] **Testes Unitários:** Cobertura mínima de 80% de testes unitários nas novas rotas criadas.
- [ ] **Integração Contínua (CI):** O build passou sem erros nas ferramentas de CI/CD (GitHub Actions) e não quebrou o ambiente de Staging.

### 2. Validação de Negócio & Produto (PO)
- [ ] **Critérios de Aceite:** Todos os cenários descritos em formato Gherkin no backlog foram validados e homologados pelo Product Owner.
- [ ] **UX/UI Review:** A interface foi validada e está de acordo com o protótipo e padrões de responsividade mobile-first.

### 3. Segurança & LGPD / RGPD
- [ ] **Mascaramento de Dados:** Dados sensíveis de alunos e professores estão criptografados na base de dados (PostgreSQL/Redis).
- [ ] **Consentimento Explicícito:** O fluxo de cadastro possui as caixas de aceite de termos de privacidade ativas e auditáveis logguadas no sistema.

### 4. Documentação Técnica
- [ ] **Swagger/OpenAPI:** As rotas criadas (ex: autenticação, progresso) foram documentadas na especificação de API.
- [ ] **Webhooks:** Os payloads JSON de disparo para integrações (ex: n8n) foram validados com a estrutura homologada no arquivo `edupath-sync.md`.

---

## 🛡️ Governança de Homologação

Se qualquer um dos itens acima falhar, o item retorna imediatamente para a coluna de **In Progress** ou **QA** no ClickUp, impedindo o deploy em produção e garantindo a estabilidade do ecossistema EduPath.
