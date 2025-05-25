# 📋 Projeto FAPG - Sprint 3

Sistema de gerenciamento de projetos da FAPG (Fundação de Apoio à Pesquisa de Pós-Graduandos), contemplando backend, frontend e banco de dados, com foco em funcionalidades administrativas para coordenadores.

---

## 📅 Sprint 3 - Entregas de 05/05 até 25/05

Durante a Sprint 3, o time se concentrou em expandir as funcionalidades de gestão da plataforma, reforçando a segurança, a usabilidade e a robustez das regras de negócio, incluindo:

- Criação de recurso para recuperação de senha
- Atribuição de responsável pela atividade, e pessoas associadas a atividade
- Aclopamento de documentos como um recurso interno de projetos, atividades e tarefas
- Acoplamento de tarefas como um recurso interno de atividades
- Implementação de regras de negócios para impedir criar tarefas com custo acima do permitido
- Implementaçaõ de regras de negócios para impedir que tarefas possuam datas fora do período definido pela atividade
- Filtro de busca por data (ínicio e fim)
- Autorização de usuários por tipo de acesso
- Intgração de IA

---

## 🎯 Objetivos da Sprint

- Recuperação de senha ✔️
- Responsável pela atividade ✔️
- Documentos ✔️
- Tarefas e controle de orçamentos ✔️
- Filtro de busca por datas ✔️
- Controle de orçamentos e prazos em atividades e tarefas ✔️
- Autorização de usuários ✔️
- Integração de IA ✔️

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





---

## 📊 Métricas do Time

O andamento das tarefas pode ser visto observando o gráfico Burndown inserido abaixo.

[AGUARDANDO O ENVIO DO GRÁFICO]

---
