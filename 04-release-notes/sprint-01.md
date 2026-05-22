# 📦 Release Notes — Sprint 1 (Fundação & Perfis)

> **Versão:** v0.1.0-mvp  
> **Data de Liberação:** Maio de 2026  
> **Status da Release:** 🔓 Produção / Homologado

## 🎯 Resumo da Entrega
Esta primeira release entrega a base estrutural e de segurança do EduPath. Focamos em garantir um ambiente blindado para o tráfego de dados e em delimitar rigidamente o que cada tipo de usuário (Professor, Aluno e RH) pode visualizar dentro do ecossistema.

---

## 🚀 Funcionalidades Incluídas

### 🔐 Sistema de Autenticação & LGPD (`ED-1 / EP-01`)
* **O que foi feito:** Criação das rotas globais de login e cadastro com criptografia de ponta a ponta.
* **Valor para o Negócio:** Garantia jurídica de conformidade com a LGPD para instituições de ensino parceiras e proteção total dos dados sensíveis dos alunos.

### 👥 Níveis de Acesso Dinâmicos (`ED-2 / EP-01`)
* **O que foi feito:** Implementação de regras de controle de acesso (RBAC). 
* **Impacto na Experiência:**
  * **Alunos** são direcionados automaticamente para a interface limpa de consumo de aulas.
  * **Coordenadores e RH** ganham permissões administrativas para edição de conteúdo e parametrização.

### 🎨 Arquitetura de Layout Base (`ED-3 / EP-07`)
* **O que foi feito:** Configuração do ecossistema de componentes visuais do front-end.
* **Valor para o Negócio:** Garante que todas as próximas telas herdará um padrão de carregamento acelerado e design unificado.

---

## 🛠️ Correções e Melhorias (Bugfixes)
* **Ajuste de Session Timeout:** Corrigido comportamento que deslogava usuários ativos em menos de 15 minutos de inatividade durante a leitura de artigos longos.
* **Sanitização de Input:** Adicionada camada de segurança extra contra SQL Injection e Cross-Site Scripting (XSS) no formulário de cadastro inicial.
