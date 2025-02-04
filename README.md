# Projeto CRUD de Estudantes com React e Node.js

Este projeto implementa um aplicativo CRUD (Create, Read, Update, Delete) simples para gerenciar dados de estudantes. Ele utiliza React para o frontend e Node.js com Express para o backend. O backend se conecta a um banco de dados MySQL para armazenar as informações dos estudantes.

## Estrutura do Projeto

O projeto está organizado em duas pastas principais:

* **frontend:** Contém o código-fonte do aplicativo React.
* **backend:** Contém o código-fonte do servidor Node.js e a lógica de acesso ao banco de dados.

## Frontend (React)

O frontend utiliza as seguintes bibliotecas:

* **React Router DOM:** Para navegação entre diferentes componentes/páginas da aplicação.
* **Axios:** Para realizar requisições HTTP ao backend.
* **Bootstrap:** Para estilização e componentes de interface do usuário.
* **React:** Biblioteca principal para construir interfaces de usuário.

**Componentes Principais:**

* **App.js:** Componente principal que configura as rotas da aplicação.
* **Student.js:** Componente que lista os estudantes, permite a exclusão e navegação para atualização.
* **CreateStudent.js:** Componente que permite a criação de novos estudantes.
* **UpdateStudent.js:** Componente que permite a atualização dos dados de um estudante existente.

## Backend (Node.js)

O backend utiliza as seguintes bibliotecas:

* **Express:** Framework web para Node.js que simplifica a criação de APIs e o roteamento de solicitações.
* **Cors:** Middleware para habilitar o Cross-Origin Resource Sharing (CORS), permitindo que o frontend acesse o backend em um domínio diferente.
* **MySQL:** Driver para interagir com o banco de dados MySQL.

**Funcionalidades da API:**

* **GET /:** Retorna todos os estudantes cadastrados.
* **POST /create:** Cria um novo estudante.
* **PUT /update/:id:** Atualiza os dados de um estudante com base no ID.
* **DELETE /student/:id:** Exclui um estudante com base no ID.

## Configuração do Banco de Dados

O backend se conecta a um banco de dados MySQL.  Certifique-se de ter o MySQL instalado e configurado em sua máquina.

**Configurações do Banco de Dados (backend/server.js):**

* **host:** "localhost"
* **user:** "root"
* **password:** ""
* **database:** "crud"

Você precisará criar um banco de dados chamado "crud" e uma tabela chamada "student" com as colunas "id" (INT, AUTO_INCREMENT, PRIMARY KEY), "name" (VARCHAR(255)) e "email" (VARCHAR(255)).

## Como Executar o Projeto

1. **Clone o repositório:** `git clone <URL_DO_REPOSITORIO>`
2. **Instale as dependências do frontend:** `cd frontend && npm install`
3. **Instale as dependências do backend:** `cd ../backend && npm install`
4. **Inicie o servidor backend:** `node server.js` (na pasta backend)
5. **Inicie o aplicativo frontend:** `npm start` (na pasta frontend)

## Tecnologias Utilizadas

* **Frontend:** React, React Router DOM, Axios, Bootstrap
* **Backend:** Node.js, Express, Cors, MySQL

## Observações

* Este README fornece uma visão geral do projeto e instruções básicas de configuração.
* Certifique-se de ter as dependências necessárias instaladas globalmente (Node.js, npm/yarn).
