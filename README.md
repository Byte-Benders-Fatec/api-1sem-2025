# 📋 Projeto FAPG - Sprint 2

Sistema de gerenciamento de projetos da FAPG (Fundação de Apoio à Pesquisa de Pós-Graduandos), contemplando backend, frontend e banco de dados, com foco em funcionalidades administrativas para coordenadores.

---

## 📅 Sprint 2 - Entregas de 07/04 até 27/04

Durante a Sprint 2, o time se concentrou em expandir as funcionalidades de gestão da plataforma, reforçando a segurança, a usabilidade e a robustez das regras de negócio, incluindo:

- Implementação de autenticação em duas etapas (2FA) via e-mail
- Criação da página de Perfil para edição de dados do usuário
- Ampliação dos vínculos entre projetos e outras entidades
- Melhorias visuais de hierarquia entre Projetos, Atividades e Tarefas
- Implementação de regras de negócio para orçamentos e prazos
- Expansão dos filtros de busca e controle de status ativo/inativo

---

## 🎯 Objetivos da Sprint

- Adição de usuários em Times ✔️
- Implementar autenticação 2FA ✔️
- CRUD completo de Instituições ✔️
- CRUD completo de Áreas ✔️
- Vincular projetos a Áreas, Times, Instituições e Agências ✔️
- Definir responsável por projeto (diferente do criador) ✔️
- Controle de orçamentos e prazos em atividades e tarefas ✔️
- Página de perfil do usuário ✔️
- Filtros de status e data para atividades ✔️

---

## ✅ Funcionalidades Implementadas

- **Backend (Node.js + Express)**:
  - Autenticação em duas etapas (envio de código de 6 dígitos por e-mail)
  - Endpoints para:
    - Instituições
    - Áreas
    - Atualização de Perfil (nome, e-mail, senha e foto de perfil)
    - Vínculo entre projetos e entidades relacionadas
    - Definição de responsável pelo projeto
    - Regras de consistência para orçamentos e datas

- **Banco de Dados (MySQL)**:
  - Novas entidades: `institution`, `area`
  - Relacionamentos para controle de vínculos entre projetos e outras entidades
  - Atualização de seeds para as novas entidades

- **Frontend (React + Vite + Tailwind)**:
  - Tela de edição de perfil do usuário
  - Tela de autenticação em duas etapas
  - CRUD completo de Instituições e Áreas
  - Edição de vínculos ao criar ou editar um Projeto
  - Melhorias visuais para Projetos > Atividades > Tarefas
  - Filtros de busca por status e data
  - Controle ativo/inativo padrão nos cadastros de Times, Usuários, Projetos, Atividades, Instituições, Áreas, Agências e Documentos

---

## 📦 Tecnologias Utilizadas

- **Backend**: Node.js, Express, JWT, Nodemailer, MySQL2, Bcrypt, Multer
- **Frontend**: React, Vite, TailwindCSS, Lucide React, Axios
- **Banco de Dados**: MySQL

---

## 🎥 Entrega Visual (MVP)

Segue vídeo demonstrativo das funcionalidades da Sprint 2, apresentando as novas funcionalidades e melhorias implementadas:


https://github.com/user-attachments/assets/5cd98a73-fd90-445f-bbef-cd1a49fce5f8


---

## 📊 Métricas do Time

O andamento das tarefas pode ser visto observando o gráfico Burndown inserido abaixo.

[AGUARDANDO O ENVIO DO GRÁFICO]

---
