
<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/VanessaSwerts/NLW-Copa-Server?color=%2304D361">

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/VanessaSwerts/NLW-Copa-Server">

  <a href="https://github.com/VanessaSwerts/NLW-Copa-Server/commits/master">
    <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/VanessaSwerts/NLW-Copa-Server">
  </a>

   <img alt="License" src="https://img.shields.io/badge/license-MIT-brightgreen">

</p>

<h4 align="center">
	✅ NLW-Copa Server - Concluído ✅
</h4>

<p align="center">
 <a href="#-sobre-o-projeto">Sobre</a> •
 <a href="#-layout">Layout</a> •
 <a href="#-como-executar-o-projeto">Como executar</a> •
 <a href="#-estrutura-de-arquivos">Estrutura de arquivos</a> • 
 <a href="#-tecnologias">Tecnologias</a> •
 <a href="#-autores">Autores</a> •
 <a href="#user-content--licença">Licença</a>
</p>


## 💻 Sobre o projeto

10° edição da Next Level Week, onde na trilha Ignite, construimos o backend e front-end (web e mobile) de um bolão da copa do mundo.

[Rocketseat](https://rocketseat.com.br/)

---

## 🎨 Diagrama Entidade Relacionamento

![Captura de tela 2022-11-06 213048](https://user-images.githubusercontent.com/57146734/200204360-7f01555c-1fcc-43b2-a6e3-89c8bea4102b.png)

---

## 🚀 Como executar o projeto

Este projeto é dividido em três partes:
1. [Frontend - Web](https://github.com/VanessaSwerts/NLW-Copa-App)
2. [Frontend - Web](https://github.com/VanessaSwerts/NLW-Copa-Web)
3. Backend (Neste repositório)

### Pré-requisitos

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[Git](https://git-scm.com) e [Node.js](https://nodejs.org/en/).

#### Executando o projeto

##### 🧭 Rodando a aplicação Backend

   ```bash
    # Clone este repositório
    $ git clone https://github.com/VanessaSwerts/NLW-Copa-Server.git

    # Acesse a pasta do projeto no seu terminal/cmd
    $ cd NLW-Copa-Server

    # Instale as dependências
    $ npm install

    # Execute a aplicação
    $ npm run dev 
    
    # O servidor irá rodar em http://localhost:3333
    
   ```

##### 🧭 Criando novo banco de dados

   ```bash   
    
    # Execute o comando
    $ npx prisma init --datasource-provider SQLite   
    
    # Execute comando para rodar as migrations
    $ npx prisma migrate dev

    # Para visualizar o banco de dados
    $ npx prisma studio
    
    # Acesse http://localhost:5555
    
   ```

---

## 📁 Estrutura de arquivos

Atualizado 06/11/2022

```
nlw-copa-server
├─ .gitignore
├─ package-lock.json
├─ package.json
├─ prisma
│  ├─ dev.db
│  ├─ ERD.svg
│  ├─ migrations
│  │  ├─ 20221102161250_create_table_pools
│  │  │  └─ migration.sql
│  │  ├─ 20221102225207_create_db_structure
│  │  │  └─ migration.sql
│  │  ├─ 20221106162151_update_poll_table
│  │  │  └─ migration.sql
│  │  ├─ 20221106165303_add_google_id_to_user_table
│  │  │  └─ migration.sql
│  │  ├─ 20221106184509_add_uniqueconstraint_on_particpant_and_game_id
│  │  │  └─ migration.sql
│  │  └─ migration_lock.toml
│  ├─ schema.prisma
│  └─ seed.ts
├─ src
│  ├─ @types
│  │  └─ fastify-jwt.d.ts
│  ├─ lib
│  │  └─ prisma.ts
│  ├─ plugins
│  │  └─ authenticate.ts
│  ├─ routes
│  │  ├─ auth.ts
│  │  ├─ game.ts
│  │  ├─ guess.ts
│  │  ├─ poll.ts
│  │  └─ user.ts
│  └─ server.ts
└─ tsconfig.json

```

---

## 🛠 Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:

#### **API**  ([Node JS](https://nodejs.org/docs/latest/api/))
- **Dependências**:
  -   **[@fastify/cors](https://github.com/fastify/fastify-cors)**
  -   **[@fastify/jwt](https://github.com/fastify/fastify-jwt)**
  -   **[@prisma/client](https://www.prisma.io/docs/concepts/components/prisma-client)**
  -   **[Fastify](https://www.fastify.io)**
  -   **[Short Unique Id](https://github.com/simplyhexagonal/short-unique-id)**
  -   **[Zod](https://github.com/colinhacks/zod)**
  
- **Dependências de Desenvolvimento**:
  -   **[Mermaid JS - Mermaid CLI](https://github.com/mermaid-js/mermaid-cli)**
  -   **[Prisma](https://www.prisma.io)**
  -   **[Prisma ERD Generator](https://github.com/keonik/prisma-erd-generator)**
  -   **[TSX](https://github.com/esbuild-kit/tsx)** 
  -   **[Typescript](https://www.typescriptlang.org)** 


Veja o arquivo  [package.json](https://github.com/VanessaSwerts/NLW-Copa-Server/blob/master/package.json)

---

## 🦸 Autores

<table>
  <tr>
    <td align="center"><a href="https://github.com/vanessaSwerts/"><img style="border-radius: 50%;" src="https://avatars2.githubusercontent.com/u/57146734?v=4" width="100px;" alt=""/><br /><sub><b>Vanessa Swerts</b></sub></a></td>
  </tr>
</table>

---

## 📝 Licença

Este projeto esta sobe a licença [MIT](./LICENSE).
