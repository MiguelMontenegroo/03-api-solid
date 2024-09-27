# App

Gympass style app.

## RFs(Requisitos funcionais)

-[x] Deve ser possível se cadastrar;
-[x] Deve ser possível se autenticar;
-[x] Deve ser possível obter o perfil de um usuário logado;
-[x] Deve ser possível obter o número de check-ins realizados pelo usuário logado;
-[x] Deve ser possível o usuário obter o seu histórico de check-ins;
-[x] Deve ser possível o usuário buscar academias próximas (até 10km);
-[x] Deve ser possível o usuário buscar uma academias pelo nome;
-[x] Deve ser possível o usuário realizar chek-in em uma academia;
-[x] Deve ser possível validar o check-in de um usuário;
-[x] Deve ser possível cadastrar uma academia;

## RNs(Regras de negócio)

- [x] O usuário não deve poder se cadastrar com um e-mail duplicado;
- [x] O usuário não pode fazer 2 check-ins no mesmo dia;
- [x] O usuário não pode fazer check-in se não estiver perto (100m) da academia;
- [x] O check-in só pode ser validado até 20 minutos após criado;
- [x] O check-in só pode ser validado por administradores;
- [x] A academia só pode ser cadastrada por administradores;

# RNFs(Requisitos não-funcionais)

- [x] A senha do usuário precisa estar criptografada;
- [x] Os dados da aplicação precisam estar persistidos em um banco PostgreSQL;
- [x] Todas listas de dados precisam estar paginadas com 20 itens por página;
- [x] O usuário deve ser identificado por um JWT (JSON Web Token);

tecnologias utilizadas: 
03-api-solid: tsx(pro node compreender o código typescript ele traduz pra javascript),tsup(biblioteca para criar a versão de build),zod(biblioteca validação variaveis),eslint(formatação e padronização de codigo),prisma(orm(object relational mapper) abstração de uma camada de serviço,mapear as tabelas do banco de dados para estruturas dentro do código e faz migration automatizada),Docker(conseguir subir o banco de dados PostgreSQL na nossa máquina),JSON web token(JWT)(autenticação criptografada),supertest(biblioteca que faz requisições HTTP (como GET, POST, PUT, DELETE) para os endpoints da sua API)
----------------------------------------------------------------------
Gympass-style app.

Functional Requirements (RFs)
 It must be possible to register;
 It must be possible to authenticate;
 It must be possible to get the profile of a logged-in user;
 It must be possible to get the number of check-ins made by the logged-in user;
 It must be possible for the user to get their check-in history;
 It must be possible for the user to search for nearby gyms (up to 10 km);
 It must be possible for the user to search for gyms by name;
 It must be possible for the user to check-in at a gym;
 It must be possible to validate a user's check-in;
 It must be possible to register a gym;
Business Rules (RNs)
 The user must not be able to register with a duplicate email;
 The user cannot check in twice on the same day;
 The user cannot check in if they are not near (100m) the gym;
 The check-in can only be validated up to 20 minutes after it was created;
 The check-in can only be validated by administrators;
 The gym can only be registered by administrators;
Non-Functional Requirements (RNFs)
 The user's password needs to be encrypted;
 The application's data needs to be stored in a PostgreSQL database;
 All data lists need to be paginated with 20 items per page;
 The user must be identified by a JWT (JSON Web Token);
End-to-End Test with GitHub Action

03-api-solid Technologies:

TSX (for Node to understand the TypeScript code, it translates to JavaScript),
Tsup (library for creating the build version),
Zod (library for validating variables),
ESLint (code formatting and standardization),
Prisma (ORM (Object Relational Mapper), abstracts a service layer, maps database tables to structures within the code, and performs automated migrations),
Docker (to set up the PostgreSQL database on our machine),
JSON Web Token (JWT) (encrypted authentication),
Supertest (library for making HTTP requests (such as GET, POST, PUT, DELETE) to your API endpoints).