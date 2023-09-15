-----------------------------------------------------------------------------------------

//comandos

- npm init -y
- npx tsc --init            ➡️ Criar um arquivo de configuração do TS
- npx tsc src/index.ts      ➡️ Coverter TS em JS
- npx eslint --ext --fix
- npx vitest                ➡️ Rotar teste

- npm run lint              ➡️ Padronização do codigo
- npm run test ou npm test  ➡️ Rotar teste
- npm run build             ➡️ Build do projeto

-----------------------------------------------------------------------------------------

// Dependencia de desenvolvimento 

- npm i -D typescript
- npm i -D @types/node
- npm i tsx -D
- npm i eslint @rocketseat/eslint-config -D
- npm i vitest -D
- npm i supertest -D
- npm i -D @types/supertest
- npm i tsup -D                               ➡️ Ferramenta que faz o build do TypeScript

// Dependedencia de Produção

- npm i fastify
- npm i knex sqlite3
- npm run knex -- migrate:make create-documents ➡️ Cria a tabela
- npm run knex -- migrate:latest                ➡️ Lê todas as migrations e executa-las
- npm run knex -- migrate:rollback              ➡️ Desfaz a migration que foi executada
- npm i dotenv          ➡️ Ler arquivo .env
- npm i zod             ➡️ Validação qualquer tipo de dados
- npm i @fastify/cookie ➡️ Ajuda a trabalhar com cookie

-----------------------------------------------------------------------------------------


// Links
- https://github.com/sidorares/node-mysql2  ➡️ Driver nativo
- https://knexjs.org/                       ➡️ Query Builder
- https://jestjs.io/pt-BR/                  ➡️ Ferramenta para teste
- https://vitest.dev/                       ➡️ Framework test

-----------------------------------------------------------------------------------------

// Conceito

- Runtime Type Checking ➡️ Só valida que esta dando erro quando executa a aplicação
- Static Type Checking  ➡️ valida os erros no momento que está desenvolvendo a aplicação


// Comunicação BD

- Driver nativos    ➡️ Ferramneta, biblioteca de baixo nivel
- Query Builder     ➡️ Construdor de query, facilita a escrita do SQL 
- ORM               ➡️

// Migrations

- Controle de versão dentro do banco de dado
- Historico de todas as mudança dentro do banco de dado
- Cria uma table e anota quais itens do historico da alteração do BD já teve


-----------------------------------------------------------------------------------------

// Requisitos Funcionais

- [x] Quais são as aplicações, o usuário pode ou não fazer dentro do APP
- [x] O usuário deve poder criar uma nova transação
- [x] O usuário deve poder um resumo da sua conta
- [x] O usuário deve poder listar todas transações que já ocorreram
- [x] O usuário deve poder visualizar uma transação única

// Regra de negocio

- [] Coisas que podem acontecer e que a aplica vai validar
- [] A transação pode ser do tipo crédito que somará ao valor total, ou débito subtrairá
- [] Deve ser possível identificarmos o usuário entre as requisições
- [] O usuário só pode visualizar transações o qual ele criou

// Requisitos não funcionais

- 

-----------------------------------------------------------------------------------------

// Request Body

- Informações que geralmente são interpretada por um protocolo HTTPs
- Informações usada geralmente para criar ou editar algum recurso 
-----------------------------------------------------------------------------------------

// Definição de tipos @types (extensão arquivo.d.ts)

- É um arquivo que não vai ter código JS dentro apenas código TS

// Cookies 

- Formas de manter contexto entre requisições

// hook

- sdasdasd?
/*
 app.addHook('preHandler', async (request) => {
    console.log(`[${request.method}] ${request.url}`)
  })
*/

-----------------------------------------------------------------------------------------

// Testes automatizados

- Formas de manter confiança na hora de dar manutenção no código a longo prazo
- Garantir que a aplicação esteja funcionando
- Da confiaça para trabalhar no código
- Assegura que todas as funcionalidade da aplicação estão funcionando

// Tipos de Testes

# Unitários

- Testa exclusivamente uma unidade da sua aplicação 

# intergração

- Testa a comunicação entre duas ou mais unidades 
- Como que varios pedaços da aplicação funciona quando estão trabalhando junto

# e2e - ponta a ponta 

- Teste que simula um usuário operando a aplicação
    - Front-end: abre a página de login, digite o texto smooth@exemplo.com no campo com ID email, click no botão

- Verifica se as porta de entrada da aplicação Back-end estão funcionando de ponta a ponta
    - Back-end: chmadas HTTP, websockets

-----------------------------------------------------------------------------------------

// Pirâmide de testes: Explica a importancia e qual teste fazer primeiro

- Primeiro a aprender: E2E (não dependem de nenhuma teecnoligia, não dependem de arquitetura)

-----------------------------------------------------------------------------------------
// Espeta em um teste 

- Em um ambiente que não tenha interferencia externa
-----------------------------------------------------------------------------------------

// Deploy - Serviço gerenciado

- Usar um serviço que automatiza as coisas
- 

-----------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------
