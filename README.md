<h1 align="center">Sistema Intuitivo para Gestão de Projetos de Pesquisa e Desenvolvimento Tecnológico de uma Fundação</h1>

## :bookmark_tabs: Índice
- [:scroll: Descrição](#scroll-descrição)
- [:memo: Backlog do Produto](#memo-backlog-do-produto)
- [:dart: Requisitos Funcionais](#dart-requisitos-funcionais)
- [:pushpin: Requisitos Não Funcionais](#pushpin-requisitos-não-funcionais)
- [:hammer_and_wrench: Tecnologias Utilizadas](#hammer_and_wrench-tecnologias-utilizadas)
- [:building_construction: MPV](#building_construction-mpv)
- [:busts_in_silhouette: Equipe](#busts_in_silhouette-equipe)
- [:calendar: Calendário API](#calendar-calendário-api)

## :scroll: Descrição
A FAPG enfrenta desafios para gerenciar os seus projetos, portanto, necessita de uma solução que simplifique e otimize esse processo. Dentre as funcionalidades mais relevantes destaca-se cadastrar os projetos e as atividades a ele correlatas, previstas em cronograma. Também é relevante que o coordenador e os demais envolvidos tenham visibilidade do andamento do projeto. A atualização do andamento das atividades previstas e seu respectivos responsáveis, dispostas em um
cronograma, bem como visualizações, são funcionalidades necessárias para acompanhar seu andamento.
Portanto, o principal objetivo deste projeto é o desenvolvimento de um sistema web intuitivo que permita a gestão de projetos e suas atividades a fim de garantir eficiência e transparência no seu acompanhamento pelos partícipes.

:link: [(Voltar ao topo)](#bookmark_tabs-índice)

## :memo: Backlog do Produto

| **Rank** | **Prioridade** | **User Story** | **Estimativa** | **Sprint** | **Requisito do Parceiro** | **Cenário de teste 1** | **Cenário de teste 2** | **Cenário de teste 3** | 
|----------|----------------|----------------|----------------|------------|---------------------------|------------------------|------------------------|------------------------| 
| 1 | Alta           | Como coordenador, eu quero cadastrar um novo projeto na plataforma para que eu possa gerenciar suas atividades e progresso. | 8 horas | Sprint 1 | Cadastrar projetos da FAPG | O sistema deve permitir a inserção de dados do projeto, como nome, descrição e área de atuação, e salvar corretamente no banco de dados. | - | - | 
| 2 | Alta           | Como coordenador, eu quero cadastrar, atualizar e excluir usuários na plataforma. | 9 horas | Sprint 1 | Cadastrar, editar e excluir usuários | O sistema deve permitir a criação, atualização e exclusão de usuários. | - | - | 
| 3 | Alta           | Como coordenador, eu quero cadastrar, atualizar e excluir times, além de poder adicionar usuários nos times criados. | 5 horas | Sprint 1 | Cadastrar, editar e excluir equipes | O sistema deve permitir a criação, edição e exclusão de times caso não sejam mais necessários, além de poder adcionar usuários em novos times. | - | - | 
| 4 | Alta           | Como coordenador, eu quero atualizar os dados de um projeto para manter as informações sempre atualizadas. | 4 horas | Sprint 1 | Atualizar dados dos projetos | O sistema deve permitir a edição de projetos já cadastrados, com os dados atualizados refletindo na visualização. | - | - | 
| 5 | Alta           | Como coordenador, eu quero excluir um projeto caso ele seja cancelado ou não seja mais necessário. | 3 horas | Sprint 1 | Excluir projetos da FAPG | O sistema deve permitir a exclusão de projetos, removendo-os permanentemente da plataforma. | - | - | 
| 6 | Alta           | Como usuário, eu quero que a interface do sistema seja intuitiva e fácil de usar para que eu não precise de treinamentos complexos. | 12 horas | Sprint 1 | Usabilidade | O sistema deve ter uma interface limpa, amigável e fácil de navegar, sem necessidade de instruções detalhadas. | - | - | 
| 7 | Alta           | Como um usuário, quero poder atualizar meus dados pessoais e minha foto de perfil, para manter minhas informações corretas e atualizadas no sistema. | 5 horas | Sprint 2 | Página de Perfil (alterar senha, mudar nome, e-mail, adicionar foto) | • Dado que estou na página de perfil, quando altero o nome e salvo, então o nome deve ser atualizado. | • Dado que desejo alterar a senha, quando informo senha atual incorreta, então deve exibir erro. | • Dado que quero adicionar uma foto, quando envio arquivo inválido, então deve impedir e alertar. | 
| 8 | Alta           | Como criador ou administrador de um time, quero adicionar ou remover integrantes, para gerenciar dinamicamente meu time. | 8 horas | Sprint 2 | Adicionar/remover integrantes ao criar ou editar um time | • Dado que estou criando um time, quando adiciono um integrante, então ele deve aparecer na lista. | • Dado que já há integrantes, quando removo um integrante, então ele não deve mais aparecer. | • Dado que estou adicionando, quando tento adicionar o mesmo usuário, então deve alertar duplicidade. | 
| 9 | Alta           | Como administrador do sistema, quero criar, editar e excluir instituições, para manter o cadastro atualizado. | 4 horas | Sprint 2 | CRUD de Instituições | • Dado que estou na página, quando crio uma instituição válida, então ela aparece na lista. | • Dado que edito uma instituição, quando salvo, então as alterações aparecem. | • Dado que excluo uma instituição, quando salvo, então ela desaparece da lista. | 
| 10 | Alta           | Como administrador do sistema, quero criar, editar e excluir áreas, para organizar melhor os projetos. | 4 horas | Sprint 2 | CRUD de Áreas | • Dado que estou na seção de Áreas, quando crio uma nova, então ela aparece listada. | • Dado que edito uma área existente, quando salvo, então o novo nome aparece. | • Dado que tento excluir uma área vinculada, então o sistema deve impedir. | 
| 11 | Alta           | Como responsável pela criação de projetos, quero vincular ou desvincular Áreas, Times, Instituições e Agências, para estruturar corretamente o projeto. | 4 horas | Sprint 2 | Vínculos entre projeto e entidades | • Dado que estou criando um projeto, quando vinculo entidades, então vínculos são salvos. | • Dado que projeto já possui vínculos, quando removo um, então não aparece mais. | • Dado que salvo sem vínculos obrigatórios, então deve alertar. | 
| 12 | Alta           | Como criador de um projeto, quero poder definir outro usuário como responsável, para delegar a gestão. | 3 horas | Sprint 2 | Definir responsável pelo projeto | • Dado que estou criando um projeto, quando escolho outro responsável, então é salvo. | • Dado que edito um projeto, quando troco o responsável, então é atualizado. | • Dado que escolho um usuário inativo, então deve impedir. | 
| 13 | Alta           | Como usuário visualizando um projeto, quero ver claramente as atividades vinculadas, para entender a estrutura. | 5 horas | Sprint 2 | Acoplamento visual de atividades ao projeto | • Dado que crio atividade, quando associo ao projeto, então ela aparece nele. | • Dado que edito uma atividade, quando salvo, então mantém associação. | • Dado que acesso o projeto, quando visualizo, então vejo apenas atividades relacionadas. | 
| 14 | Alta           | Como usuário gerenciando atividades, quero filtrar por status e data, para localizar atividades específicas. | 4 horas | Sprint2 | Filtro de busca de atividades por status e data | • Dado que filtro por status, quando aplico, então só vejo atividades com aquele status. | • Dado que filtro por data, quando aplico, então só vejo atividades no intervalo. | • Dado que combino filtros, quando aplico, então só vejo atividades que atendem ambos critérios. | 
| 15 | Alta           | Como gestor de projetos, quero garantir que as atividades respeitem o período do projeto, para manter consistência. | 4 horas | Sprint 2 | Regras de datas das atividades | • Dado que crio uma atividade, quando datas estão corretas, então atividade é salva. | • Dado que inicio atividade antes do projeto, quando tento salvar, então erro ocorre. | • Dado que término é após o projeto, quando salvo, então sistema impede. | 
| 16 | Alta           | Como gestor financeiro do projeto, quero que as atividades respeitem o orçamento, para evitar ultrapassá-lo. | 3 horas | Sprint 2 | Regras de orçamento de atividades | • Dado que o orçamento permite, quando crio atividade, então ela é salva. | • Dado que orçamento estoura, quando crio nova atividade, então sistema impede. | • Dado que aumento orçamento em edição, quando excede, então sistema bloqueia.| 
| 17 | Média          | Como usuário visualizando uma atividade, quero ver claramente as tarefas vinculadas, para entender a estrutura e progresso. | 10 horas | Sprint 3 | Acoplamento de tarefas a atividades | • Dado que crio tarefa em uma atividade, quando salvo, então tarefa aparece vinculada. | • Dado que edito uma tarefa, quando salvo, então mantém associação à atividade. | • Dado que visualizo uma atividade, quando acesso, então vejo suas tarefas. | 
| 18 | Alta           | Como gestor de atividades, quero garantir que o custo da tarefa não exceda o orçamento da atividade, para manter o controle financeiro. | 10 horas | Sprint 3 | Validação de custo da tarefa (orçamento da atividade) | • Dado que custo está dentro do orçamento, quando crio tarefa, então sistema permite. | • Dado que custo excede orçamento, quando tento salvar, então sistema bloqueia. | • Dado que edito tarefa, quando novo valor excede, então sistema impede.| 
| 19 | Média          | Como usuário, quero que documentos estejam claramente vinculados aos projetos, atividades ou tarefas, para fácil organização e rastreabilidade. | 15 horas | Sprint 3 | Acoplamento de documentos (projetos, atividades, tarefas) | • Dado que adiciono documento a projeto, quando salvo, então ele aparece vinculado. | • Dado que adiciono a atividade, quando visualizo, então vejo o documento listado. | • Dado que adiciono a tarefa, quando acesso, então documento aparece vinculado. | 
| 20 | Baixa          | Como usuário que esqueceu a senha, quero receber uma senha temporária por e-mail, para poder acessar novamente o sistema com segurança. | 8 horas | Sprint 3 | Recuperação de senha com envio de senha temporária | • Dado que solicito recuperação, quando informo e-mail válido, então recebo nova senha. | • Dado que recebo senha temporária, quando uso para login, então acesso é permitido. | • Dado que acesso com senha temporária, quando logado, então posso trocar por nova senha. | 
| 21 | Baixa          | Como criador ou editor de uma atividade, quero definir um responsável principal e usuários associados, para facilitar a gestão da execução. | 8 horas | Sprint 3 | Definição de responsável e pessoas associadas à atividade | • Dado que crio uma atividade, quando escolho um responsável, então ele é salvo. | • Dado que adiciono usuários associados, quando salvo, então eles aparecem vinculados. | • Dado que edito atividade, quando troco o responsável, então alteração é aplicada. | 
| 22 | Média          | Como usuário visualizando tarefas de uma atividade, quero filtrar por datas, para localizar tarefas em um intervalo específico. | 8 horas | Sprint 3 | Filtro por data nas tarefas de uma atividade | • Dado que acesso lista de tarefas, quando filtro por datas, então vejo apenas tarefas no intervalo. | • Dado que removo filtros, quando atualizo, então vejo todas novamente. | • Dado que combino com outros filtros, quando aplico, então lista respeita todos os critérios. | 
| 23 | Baixa          | Como criador de tarefas, quero garantir que as datas estejam dentro do período da atividade, para manter consistência temporal. | 8 horas | Sprint 3 | Validação de datas da tarefa (período da atividade) | • Dado que defino datas válidas, quando salvo, então tarefa é criada. | • Dado que início da tarefa é anterior à atividade, quando salvo, então sistema impede. | • Dado que término da tarefa é após atividade, quando salvo, então erro é exibido. | 
| 24 | Média          | Como administrador do sistema, quero garantir que cada tipo de usuário veja e edite apenas o que lhe é permitido, para manter segurança e organização. | 10 horas | Sprint 3 | Autorização de usuários por tipo de acesso | • Dado que sou usuário comum, quando acesso área de admin, então vejo acesso negado. | • Dado que sou gestor, quando edito atividades, então sou autorizado. | • Dado que mudo tipo de usuário, quando salvo, então permissões mudam conforme esperado. | 
| 25 | Média          | Como usuário da plataforma, quero utilizar recursos de inteligência artificial para apoio na organização e automação de tarefas, para ganhar produtividade. | 15 horas | Sprint 3 | Integração de IA | • Dado que acesso IA em projeto, quando solicito sugestões, então recebo atividades recomendadas. | • Dado que estou editando tarefa, quando IA ativa, então posso preencher automaticamente. | • Dado que não tenho permissão, quando tento usar IA, então acesso é negado. | 


:link: [(Voltar ao topo)](#bookmark_tabs-índice)

## :dart: Requisitos Funcionais

| | |
|:----:|:----:|
| **RF1** | Cadastrar projetos da FAPG (nome do projeto, descrição, etc) |
| **RF2** | Permitir a recuperação de dados de projetos, de forma intuitiva |
| **RF3** | Permitir atualizar e excluir dados dos projetos |
| **RF4** | Visualizar projetos por área de atuação |
| **RF5** | Visualizar projetos por responsáveis |
| **RF6** | Visualizar projetos pelo status |
| **RF7** | Acompanhar andamento das atividades |

:link: [(Voltar ao topo)](#bookmark_tabs-índice)

## :pushpin: Requisitos Não Funcionais

| | |
|:----:|:----:|
| **RNF1** | Usabilidade |
| **RNF2** | Privacidade de dados |
| **RNF3** | Conversão de linguagem natural para chamada de funções (sem uso de API externa) |
| **RNF4** | Extração de parâmetros da mensagem do usuário (sem uso de API externa) |
| **RNF5** | Orquestrar chamadas de funções |

:link: [(Voltar ao topo)](#bookmark_tabs-índice)

## :hammer_and_wrench: Tecnologias Utilizadas
![TS](https://github.com/user-attachments/assets/3be06100-5d27-4d86-991b-ba1f36be2855) ![React](https://github.com/user-attachments/assets/7949954a-cb19-4ba4-9837-35247a5a63b9) ![Html](https://github.com/user-attachments/assets/620a2e3d-f9b4-4bbc-8076-681b3457244d) ![CSS](https://github.com/user-attachments/assets/27be157c-23a7-43bc-942a-ea9aef9f1482) ![Node](https://github.com/user-attachments/assets/1aabedf5-be97-4f0d-9dc0-bb2833a2f76c) ![MySql](https://github.com/user-attachments/assets/5729a0ba-8f23-48b3-ab4a-5baf0947e32e)

:link: [(Voltar ao topo)](#bookmark_tabs-índice)

## :building_construction: MPV

**Sprint 1**:


https://github.com/user-attachments/assets/0ee99730-6dd1-4fb4-b027-ebaa989724f2


**Sprint 2**:


https://github.com/user-attachments/assets/5cd98a73-fd90-445f-bbef-cd1a49fce5f8


**Sprint 3**:


https://github.com/user-attachments/assets/6d2361ab-e651-436d-818f-aae50cdf88a4


:link: [(Voltar ao topo)](#bookmark_tabs-índice)

## :busts_in_silhouette: Equipe 
| Nome | Função | GitHub | LinkedIn |
|:----:|:------:|:------:|:--------:|
| Diego Castro | Product Owner | [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Diegocastro5) |    [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/diegocastro91/)  |
| Henrique Bitencourt | Dev Team | [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/hriquen)||
| Joniel Oliveira | Scrum Master | [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/JonielOliveira) |     [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/jonielrodrigues)  |
| Lucas Cassiano | Dev Team | [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/LucasCassiano1) |     [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-cassiano-pontes-02b4a6301?trk=contact-info)  |
| Mariana Tebecherani | Dev Team | [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Marianatebecherani) |     [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/mariana-rebelo-tebecherani-3207a4214)  |
| Thiago Ribeiro | Dev Team | [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/yrnThiago) |     [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/thiago-ribeiro-690b4114b/)  |

:link: [(Voltar ao topo)](#bookmark_tabs-índice)


## :calendar: Calendário API

| Status | Evento | Data / Período |
|:------:|:------:|:--------------:|
| :heavy_check_mark: | Kick-off Geral | 24/02 a 28/02 |
| :heavy_check_mark: | Sprint 1 | 10/03 a 30/03 |
| :heavy_check_mark: | Sprint Review / Planning | 31/03 a 04/04 |
| :heavy_check_mark: | Sprint 2 | 07/04 a 27/04 |
| :heavy_check_mark: | Sprint Review / Planning| 28/04 a 02/05 |
| :heavy_check_mark: | Sprint 3 | 05/05 a 25/05 |
| :arrow_right: | Sprint Review | 26/05 a 30/05 |
| :hourglass_flowing_sand: | Feira de Soluções | 17/06 |

:link: [(Voltar ao topo)](#bookmark_tabs-índice)
