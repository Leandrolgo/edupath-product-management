# ⚙️ Acordos de Qualidade (DoR & DoD) — EduPath

Para garantir a eficiência, alinhar as expectativas do time de engenharia e mitigar bugs ou retrabalho, o ciclo de vida de todas as histórias de usuário do EduPath segue estritamente os critérios descritos abaixo.

---

## 🟢 Definition of Ready (DoR) — Definição de Pronto para Desenvolvimento

Uma história de usuário só será puxada para a Sprint (colocada na coluna *To Do*) se cumprir **100%** dos requisitos abaixo durante a reunião de Refinamento (Refinement):

1. **Formato Padrão:** A história deve estar escrita sob a ótica da persona mapeada (`Como [Persona]... Quero [Funcionalidade]... Para [Valor de Negócio]...`).
2. **Critérios de Aceite:** Deve conter limites claros de comportamento do sistema, especificando cenários positivos e negativos descritos de forma testável.
3. **Dependências Mapeadas:** Quaisquer impedimentos técnicos, APIs de terceiros ou integrações necessárias devem estar identificados e resolvidos.
4. **Design / Protótipo Anexado:** O link ou print dos ecrãs de interface (Figma, Miro ou esquemáticos de UI) deve estar anexado à tarefa.
5. **Estimativa Técnica:** O time de engenharia deve ter debatido a complexidade e atribuído os Story Points utilizando a sequência de Fibonacci (Planning Poker).

---

## 🔵 Definition of Done (DoD) — Definição de Concluído

Uma história de usuário só será movida para a coluna *Done* (Concluído) e contabilizada como entrega da Sprint se passar com sucesso por todas as seguintes etapas:

1. **Revisão de Código (Peer Review):** O código deve ter sido revisado e aprovado por pelo menos um outro engenheiro de software (Pull Request aprovado no GitHub).
2. **Ambiente de Homologação (Staging):** A funcionalidade deve estar publicada no ambiente de testes, sem quebrar nenhuma regra legada de regressão.
3. **Testes Automatizados e Manuais:** * Cobertura mínima de testes unitários executada com sucesso.
   * Validação dos critérios de aceite executada manualmente.
4. **Homologação do Product Owner:** O PO (Leandro) deve testar a funcionalidade no ambiente de testes e validar se ela atende fielmente às regras de negócio desenhadas.
5. **Documentação Atualizada:** Quaisquer novas rotas de API, tabelas no banco de dados ou configurações do sistema devem ser documentadas na wiki do projeto.
