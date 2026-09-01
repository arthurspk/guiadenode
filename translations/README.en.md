<p align="center">
  <a href="https://github.com/arthurspk/guiadevbrasil">
    <img src="../images/guia.png" alt="Guia Dev Brasil" width="160" height="160">
  </a>
  <h1 align="center">Node.js Guide</h1>
</p>

<p align="center">
  <img src="https://img.shields.io/github/stars/arthurspk/guiadenode?style=flat-square" alt="Stars">
  <img src="https://img.shields.io/github/forks/arthurspk/guiadenode?style=flat-square" alt="Forks">
  <img src="https://img.shields.io/github/last-commit/arthurspk/guiadenode?style=flat-square" alt="Last commit">
  <img src="https://img.shields.io/github/license/arthurspk/guiadenode?style=flat-square" alt="License">
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat-square" alt="PRs Welcome">
</p>

> Complete Node.js guide: learning paths, courses, books, channels, tools and communities
> to get into the field and grow. Last review: September 2026.
>
> This is a translation of the Brazilian Portuguese guide. Resources are curated for the Brazilian community, so many are in Portuguese; 🇺🇸 marks English-language content.

## 🌍 Languages
[🇧🇷 Português](../README.md) · 🇺🇸 English (you are here)

## 📚 Table of contents
- [🎯 About this guide](#-about-this-guide)
- [🗺️ Roadmap](#️-roadmap)
- [🚀 Where to start](#-where-to-start)
- [🎓 Free courses](#-free-courses)
- [💰 Paid courses](#-paid-courses)
- [📖 Documentation](#-documentation)
- [📚 Books](#-books)
- [🎥 YouTube channels](#-youtube-channels)
- [🎙️ Podcasts](#️-podcasts)
- [📰 Sites, blogs and newsletters](#-sites-blogs-and-newsletters)
- [🛠️ Tools](#️-tools)
- [🧪 Hands-on projects and challenges](#-hands-on-projects-and-challenges)
- [🤖 AI in practice](#-ai-in-practice)
- [📜 Certifications](#-certifications)
- [💼 Career and jobs](#-career-and-jobs)
- [👥 Communities](#-communities)
- [🚨 How to contribute](#-how-to-contribute)
- [📄 License](#-license)
- [💙 Support the project](#-support-the-project)

## 🎯 About this guide
Node.js is the environment that runs **JavaScript outside the browser**: created in 2009 on top of Chrome's V8 engine and maintained today by the OpenJS Foundation, it powers APIs, websites, command-line tools, bots and the tooling of practically the whole web ecosystem (npm, bundlers, frameworks). Its asynchronous, event-driven model serves many connections at once with few resources — which is why it is the most requested back-end technology in JavaScript job posts in Brazil.

Node.js in 2026 is quite different from a few years ago: version **24 is the active LTS** (22 is in maintenance, 20 reached end of life in April and **26** becomes LTS in October), and things that used to require libraries now ship built in — `fetch`, `node --test`, `node --watch`, `--env-file`, `node:sqlite`, **native TypeScript execution** (type stripping) and the **permission model** (`--permission`).

This guide is for people who already know (or are learning) JavaScript and want to use Node.js to build back-ends and tools, from `node hello.js` to deployment. **Portuguese and free** resources come first in every section; 💰 marks paid content, 🇺🇸 English-language content and 🆕 material published or updated between 2024 and 2026. Every link was verified on the date of the last review.

## 🗺️ Roadmap
- [roadmap.sh — Node.js Developer Roadmap](https://roadmap.sh/nodejs) — Community-made visual, interactive roadmap: core modules, npm, frameworks, testing, deployment — with links per topic. 🇺🇸
- [roadmap.sh — Backend Developer Roadmap](https://roadmap.sh/backend) — The full back-end path (HTTP, databases, APIs, caching, security) that Node.js fits into. 🇺🇸
- [Introduction to Node.js (Node.js Learn)](https://nodejs.org/learn/getting-started/introduction-to-nodejs) — Official page explaining what Node.js is, why it is asynchronous and how to run your first server. 🇺🇸
- [Sobre o Node.js (site oficial em português)](https://nodejs.org/pt-br/about) — Official translated presentation: event-driven model, non-blocking I/O and an HTTP server example.
- [Node.js Reference Architecture (Red Hat e IBM)](https://nodeshift.dev/nodejs-reference-architecture/) — Opinions from two teams running Node.js in production: which packages and practices to pick for each need. 🇺🇸

**Summary path** (follow in order; each step has resources in the sections below):

1. **Modern JavaScript (ES6+)** — `let/const`, arrow functions, destructuring, ES modules, `Promise`/`async-await`. Without this, Node.js will just look like "callback errors".
2. **Runtime fundamentals** — install the LTS version, `node`/`npm`/`npx`, `package.json`, CommonJS × ESM modules, the event loop and why I/O is asynchronous.
3. **Core modules** — `fs`, `path`, `http`, `events`, `stream`, `child_process`, `process`, `fetch`, `node:test`.
4. **HTTP APIs** — REST with Express or Fastify: routes, middleware, validation (Zod), error handling, authentication (JWT).
5. **Data** — PostgreSQL or MongoDB with an ORM/ODM (Prisma, Drizzle, Mongoose), migrations, environment variables.
6. **Quality** — tests (`node --test`, Vitest or Jest), ESLint/Biome, TypeScript, structured logs (Pino), debugging with `--inspect`.
7. **Production** — Docker, PM2 or containers, deployment (Render, Railway, Fly.io), security (Helmet, `npm audit`, Permission Model), monitoring.
8. **Advanced** — streams and backpressure, workers and cluster, queues (BullMQ), WebSockets, architecture (Clean Architecture, NestJS), performance (Clinic.js, autocannon), contributing to core.

## 🚀 Where to start
1. **Master JavaScript first.** Use the [MDN JavaScript Guide](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript) or [Matheus Battisti's JavaScript 2024 course](https://www.youtube.com/playlist?list=PLnDvRpP8BnexyabTa4NQrLy3s5NowwAxb) (Portuguese) — Node.js is JavaScript underneath.
2. **Install the LTS version** from the [official download page](https://nodejs.org/pt-br/download) (or with [nvm](https://github.com/nvm-sh/nvm)/[fnm](https://github.com/Schniz/fnm) to switch versions) and [Visual Studio Code](https://code.visualstudio.com/).
3. **Understand what Node is** by reading the [official introduction](https://nodejs.org/learn/getting-started/introduction-to-nodejs) and [Alura's article on the event loop](https://www.alura.com.br/artigos/arquitetura-node-js-entenda-loop-de-eventos) (Portuguese).
4. **Take a quick course:** [Felipe Rocha](https://www.youtube.com/watch?v=IOfDoyP1Aq0) (single lesson) or [Stack Mobile's Node.js 2025 course](https://www.youtube.com/playlist?list=PLizN3WA8HR1w14FUaPYsP9q1nBHuTa1Dv) (both in Portuguese).
5. **Go deeper with a full course:** [Matheus Battisti's Node.js](https://www.youtube.com/playlist?list=PLnDvRpP8BneyHealXbzntUoFtE4SrFWWW) or, if you already want TypeScript, [From zero to production (Waldemar Neto)](https://www.youtube.com/playlist?list=PLz_YTBuxtxt6_Zf1h-qzNsvVt46H8ziKh).
6. **Build your first API** following the [MDN Express tutorial](https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Extensions/Server-side/Express_Nodejs) and test it with [Bruno](https://www.usebruno.com/) or [Hoppscotch](https://hoppscotch.io/).
7. **Write tests early** with the [built-in test runner](https://nodejs.org/learn/test-runner/using-test-runner) — nothing to install.
8. **Publish a project** on GitHub and online ([Render](https://render.com/) or [Railway](https://railway.com/)); then take on a [backend-br](https://github.com/backend-br/desafios) challenge or the [Rinha de Backend](https://github.com/zanfranceschi/rinha-de-backend-2025).

Your first server in 30 seconds (without installing any package):

```bash
mkdir hello-node && cd hello-node
npm init -y
```

```js
// server.js
import { createServer } from "node:http";

createServer((req, res) => {
  res.setHeader("Content-Type", "application/json; charset=utf-8");
  res.end(JSON.stringify({ message: "Hello, Guia Dev Brasil!" }));
}).listen(3000, () => console.log("http://localhost:3000"));
```

```bash
node --watch server.js          # restarts by itself when the file changes
```

```js
// server.test.js
import { test } from "node:test";
import assert from "node:assert/strict";

test("responds with JSON", async () => {
  const res = await fetch("http://localhost:3000");
  assert.equal((await res.json()).message, "Hello, Guia Dev Brasil!");
});
```

```bash
node --test                     # built-in test runner (with the server running)
node server.ts                  # Node.js 22.18+/24 runs TypeScript directly (type stripping)
node --permission --allow-fs-read=. server.js     # permission model
```

> Tip: to use `import` as above, add `"type": "module"` to `package.json` or save the files as `.mjs`.

## 🎓 Free courses
### In Portuguese
- [Curso de Node.js 2025 — Iniciante (Stack Mobile)](https://www.youtube.com/playlist?list=PLizN3WA8HR1w14FUaPYsP9q1nBHuTa1Dv) — Recent free playlist for people who have never done back-end: install, modules, API and database. 🆕
- [Curso de Node.js Para Completos Iniciantes (Felipe Rocha)](https://www.youtube.com/watch?v=IOfDoyP1Aq0) — Single, didactic lesson: what Node is, npm, Express and your first API in a few hours.
- [Node.js (Matheus Battisti — Hora de Codar)](https://www.youtube.com/playlist?list=PLnDvRpP8BneyHealXbzntUoFtE4SrFWWW) — Hora de Codar playlist covering Node.js from the basics to projects with Express and MongoDB.
- [Repositório do curso Node.js completo (Hora de Codar)](https://github.com/matheusbattisti/node_completo) — Source code for the lessons of Matheus Battisti's Node.js course.
- [Autenticação com Node.js e MongoDB com JWT (Matheus Battisti)](https://www.youtube.com/watch?v=qEBoZ8lJR3k) — Complete login and sign-up with JWT, from scratch — a topic that shows up in every back-end interview.
- [Curso de Node.js (Victor Lima — Guia do Programador)](https://www.youtube.com/playlist?list=PLJ_KhUnlXUPtbtLwaxxUxHqvcNQndmI4B) — Classic free video course, from "what is Node" to apps with Express and a database.
- [Curso de Node (CFBCursos)](https://www.youtube.com/playlist?list=PLx4x_zx8csUjFC41ev2qX5dnr-0ThpoXE) — Short, sequential lessons by Bruno Campagnolo: install, modules, server and routes.
- [Do zero a produção: API Node.js com TypeScript (Waldemar Neto)](https://www.youtube.com/playlist?list=PLz_YTBuxtxt6_Zf1h-qzNsvVt46H8ziKh) — Real-world project with TypeScript, tests (Jest/TDD), continuous integration and deployment.
- [Curso de API Rest, Node e TypeScript (Lucas Souza Dev)](https://www.youtube.com/playlist?list=PL29TaWXah3iaaXDFPgTHiFMBF6wQahurP) — Building a complete API from scratch, with validation, database, authentication and tests.
- [Criando APIs com NodeJs (balta.io)](https://www.youtube.com/playlist?list=PLHlHvK2lnJndvvycjBqQAbgEDqXxKLoqn) — Free balta.io course: REST API with Node, Express and MongoDB, step by step.
- [Curso NodeJS com TypeScript (Andrew Rosário)](https://www.youtube.com/playlist?list=PLn3kOoc0oI2cQDdUEQxj75sxgRH53DmSc) — Node + TypeScript environment set up from scratch, with a practical API.
- [Curso de Node.js com Express, Sequelize e Postgres (Prof. Jesiel Viana)](https://www.youtube.com/playlist?list=PLAxN8g6Knm0camfON299B-vl31IYQhA8Q) — Complete app with a relational database (PostgreSQL) and ORM, with a vanilla JavaScript front-end.
- [Mini curso de Node.js (Celke)](https://www.youtube.com/playlist?list=PLmY5AEiqDWwBHJ3i_8MDSszXXRTcFdkSu) — Windows install and first steps, good for people who have never opened a terminal.
- [REST API com Node.JS (Maransatto)](https://www.youtube.com/playlist?list=PLWgD0gfm500EMEDPyb3Orb28i7HK5_DkR) — Starts by explaining what a REST API is before coding — great for cementing concepts.
- [Mini Curso Node.js e TypeScript (Jorge Aluizio)](https://www.youtube.com/playlist?list=PLE0DHiXlN_qp251xWxdb_stPj98y1auhc) — Short RESTful API with Node.js and TypeScript for people who want to see the whole flow quickly.
- [API em Node.js + TS com Programação Funcional (Fernando Daciuk)](https://www.youtube.com/playlist?list=PLr4c053wuXU_2sufpBUxu3bLRBbyWt4lX) — A functional approach to Node APIs — a different angle from traditional courses.
- [Node JS Curso Básico (Programador Tech)](https://www.youtube.com/playlist?list=PLJ0IKu7KZpCRCJgiT6jL4jJgssEcTBsg7) — Fundamentals in short lessons: modules, npm, HTTP server and Express.
- [Curso de Node JS (Professor Edson Maia)](https://www.youtube.com/playlist?list=PLnex8IkmReXwCyR-cGkyy8tCVAW7fGZow) — From download and install to extra tooling, at a classroom pace.
- [Node js com Typescript (Erick Wendel)](https://www.youtube.com/watch?v=3kMnv46J2X8) — Lesson by Erick Wendel, Node.js core member, on using TypeScript with Node.
- [Recriando o Node.js do zero (Erick Wendel, BrazilJS)](https://www.youtube.com/watch?v=W-hFZC8q_AA) — Talk that shows how Node works inside (V8, libuv, event loop) by rebuilding it live.
- [NestJS do ZERO (Rocketseat)](https://www.youtube.com/watch?v=TRa55WbWnvQ) — Introduction to NestJS, the Node framework most requested in Brazilian corporate job posts.
- [GraphQL no Node.js do ZERO (Rocketseat)](https://www.youtube.com/watch?v=1dz48pReq_c) — Two complete apps with GraphQL on Node — an alternative to REST worth knowing.
- [Discover (Rocketseat)](https://app.rocketseat.com.br/journey/discover/overview) — Rocketseat's free fundamentals path, the entry point to their Node.js program.
- [Curso Node JS completo (DIO)](https://www.dio.me/curso-node-js) — DIO course from basic to advanced, free with certificate.
- [Introdução ao Node.js com JavaScript (DIO)](https://www.dio.me/courses/introducao-ao-nodejs-com-javascript) — First contact with Node at DIO, building a small memory-management app.
- [Fundamentos de Node.js e Jest (DIO)](https://www.dio.me/courses/fundamentos-de-nodejs-e-jest) — Servers, TypeScript and unit tests with Jest in a single course.
- [Debugging com Node.js (DIO)](https://www.dio.me/courses/debugging-com-nodejs) — How to use the inspector and VS Code to find bugs — a skill few courses teach.
- [Curso de Node.js Grátis (Cursa)](https://cursa.com.br/curso-de-node-js-gr%c3%a1tis/91) — Free course with certificate: Node, Express, MySQL with Sequelize and MongoDB with Mongoose.
- [Full Stack Open — Parte 3: Programando um servidor com Node.js e Express (PT-BR)](https://fullstackopen.com/ptbr/part3/) — University of Helsinki course translated into Portuguese: Express, MongoDB, validation and deployment.

### In English
- [Node.js and Express.js — Full Course (freeCodeCamp)](https://www.youtube.com/watch?v=Oe421EPjeBE) — Eight hours by John Smilga: modules, npm, Express, middleware and a complete API. 🇺🇸
- [Node.js / Express Course — Build 4 Projects (freeCodeCamp)](https://www.youtube.com/watch?v=qwfE7fSVaZM) — Four real projects (with MongoDB, authentication and deployment) to consolidate the basics. 🇺🇸
- [Node.js Full Course for Beginners — 7 Hours (Dave Gray)](https://www.youtube.com/watch?v=f2EqECiTBL8) — Complete, well-paced course with emphasis on REST, JWT authentication and MongoDB. 🇺🇸
- [Node.js Crash Course (Traversy Media, 2024)](https://www.youtube.com/watch?v=32M1al-Y6Ag) — Updated crash course with modern Node: ES modules, native HTTP server and `--watch`. 🆕 🇺🇸
- [Node.js Tutorial for Beginners: Learn Node in 1 Hour (Mosh)](https://www.youtube.com/watch?v=TlB_eWDSMt4) — The most-watched introduction on YouTube: clear, short and to the point. 🇺🇸
- [Node.js Ultimate Beginner's Guide in 7 Easy Steps (Fireship)](https://www.youtube.com/watch?v=ENrzD9HAZK4) — Overview in minutes: event loop, modules, npm and deployment. 🇺🇸
- [Node.js Tutorial (Codevolution)](https://www.youtube.com/playlist?list=PLC3y8-rFHvwh8shCMHFA5kWxD9PaPwxaY) — Long, systematic playlist explaining the core modules (fs, streams, events, http) one by one. 🇺🇸
- [Node.js Crash Course Tutorial (Net Ninja)](https://www.youtube.com/playlist?list=PL4cUxeGkcC9jsz4LDYc6kv3ymONOKxwBU) — Short series with Express, EJS and MongoDB, ideal for a first full-stack project. 🇺🇸
- [Node.js in 2022 — REST API completa sem frameworks (Erick Wendel)](https://www.youtube.com/watch?v=xR4D2bp8_S0) — API and tests using only Node's core modules — shows what frameworks hide. 🇺🇸
- [Node.js for Beginners (Microsoft Developer)](https://www.youtube.com/playlist?list=PLlrxD0HtieHje-_287YJKhY8tDeSItwtg) — Microsoft's official series in short videos: setup, modules, Express, debugging and deployment. 🇺🇸
- [Introduction to Node.js (LinuxFoundationX, edX)](https://www.edx.org/learn/node-js/the-linux-foundation-introduction-to-node-js) — Linux Foundation/OpenJS course with free access to the lessons; the certificate is paid. 🇺🇸
- [Back End Development and APIs (freeCodeCamp)](https://www.freecodecamp.org/learn/back-end-development-and-apis) — freeCodeCamp's free certification: npm, Express, MongoDB and five API projects. 🇺🇸
- [NodeJS (The Odin Project)](https://www.theodinproject.com/paths/full-stack-javascript/courses/nodejs) — Open, project-based course: Express, Prisma, authentication and APIs. 🇺🇸

## 💰 Paid courses
- [Formação Node.js (Rocketseat)](https://www.rocketseat.com.br/formacao/node) — Rocketseat's complete program: APIs with Fastify, Prisma, tests, Docker and deployment, with a Discord community. 🆕 💰
- [Formação APIs com Node.js e Express (Alura)](https://www.alura.com.br/formacao-node-js-express) — Alura learning path with a certificate recognized in the Brazilian market. 💰
- [Cursos de Node.js na Alura](https://www.alura.com.br/cursos-online-back-end/javascript-node-js) — Alura's full catalog of Node courses (Express, NestJS, testing, authentication, architecture). 💰
- [Full Cycle](https://fullcycle.com.br/) — Program on architecture, microservices and DevOps with many modules in Node.js/TypeScript. 💰
- [branas.io — Formações em Arquitetura de Software (Rodrigo Branas)](https://www.branas.io/) — Clean Code, Clean Architecture, TDD and DDD with projects in Node.js and TypeScript. 💰
- [Learn Node (Wes Bos)](https://learnnode.com/) — Premium Node, Express and MongoDB course building a real app. 💰 🇺🇸
- [Learn Node.js (Codecademy)](https://www.codecademy.com/learn/learn-node-js) — Interactive in-browser course; certificate on the Pro plan. 💰 🇺🇸

## 📖 Documentation
- [Node.js — Documentação da API (última versão)](https://nodejs.org/docs/latest/api/) — Official reference for every core module (`fs`, `http`, `stream`, `test`, `sqlite`…). Bookmark it. 🇺🇸
- [Node.js Learn (guia oficial)](https://nodejs.org/learn) — Official tutorials from basic to advanced: install, event loop, streams, testing, TypeScript, diagnostics. 🇺🇸
- [Node.js — site oficial em português](https://nodejs.org/pt-br) — Home, "About" page and downloads translated into Portuguese.
- [Node.js — Baixar (PT-BR)](https://nodejs.org/pt-br/download) — Installers and per-OS instructions, including version managers.
- [Node.js — Lançamentos e calendário de versões (PT-BR)](https://nodejs.org/pt-br/about/previous-releases) — Which version is LTS, which is Current and until when each one is supported.
- [Node.js Release Working Group](https://github.com/nodejs/Release) — Official source of the release schedule (`schedule.json`) and the LTS policy. 🇺🇸
- [Modules: TypeScript (type stripping)](https://nodejs.org/api/typescript.html) — Official docs on how Node runs `.ts` files natively by stripping types. 🆕 🇺🇸
- [Running TypeScript Natively (Node.js Learn)](https://nodejs.org/learn/typescript/run-natively) — Official guide: `node app.ts` with no build step, what works and what still needs a flag. 🆕 🇺🇸
- [Test runner (`node:test`)](https://nodejs.org/api/test.html) — Reference for the built-in test runner: `describe/it`, mocks, snapshots, coverage and `node --test`. 🆕 🇺🇸
- [Using Node.js's test runner (Node.js Learn)](https://nodejs.org/learn/test-runner/using-test-runner) — Official tutorial on organizing and running tests without installing anything. 🆕 🇺🇸
- [Command-line API (`--watch`, `--env-file`, `--permission`…)](https://nodejs.org/api/cli.html) — Every flag of the `node` executable, including watch mode and native `.env` loading. 🇺🇸
- [Permissions (Permission Model)](https://nodejs.org/api/permissions.html) — How to restrict file system, network and child-process access with `--permission`. 🆕 🇺🇸
- [SQLite nativo (`node:sqlite`)](https://nodejs.org/api/sqlite.html) — SQLite built into Node, with no dependencies — great for prototypes and CLIs. 🆕 🇺🇸
- [Modules: ECMAScript modules](https://nodejs.org/api/esm.html) — `import`/`export` in Node, interop with CommonJS and `require(esm)`. 🇺🇸
- [Single executable applications](https://nodejs.org/api/single-executable-applications.html) — Bundle your Node application into a single executable binary. 🆕 🇺🇸
- [The Node.js Event Loop (Node.js Learn)](https://nodejs.org/learn/asynchronous-work/event-loop-timers-and-nexttick) — The official text on the event loop, timers and `process.nextTick()` — required reading. 🇺🇸
- [Security Best Practices (Node.js Learn)](https://nodejs.org/learn/getting-started/security-best-practices) — Known threats (DoS, prototype pollution, supply chain) and how to mitigate them. 🇺🇸
- [Debugging Node.js (Node.js Learn)](https://nodejs.org/learn/getting-started/debugging) — How to use `--inspect`, Chrome DevTools and VS Code to debug. 🇺🇸
- [Using the Fetch API with Undici (Node.js Learn)](https://nodejs.org/learn/getting-started/fetch) — Global `fetch` in Node and the Undici HTTP client underneath it. 🆕 🇺🇸
- [Node.js 22 is now available!](https://nodejs.org/en/blog/announcements/v22-release-announce) — Official release post for 22 (LTS "Jod"): `require(esm)`, stable `--watch`, native WebSocket. 🆕 🇺🇸
- [Node.js 24.0.0 (Current)](https://nodejs.org/en/blog/release/v24.0.0) — Release notes for 24 (LTS "Krypton", the active LTS in 2026). 🆕 🇺🇸
- [Node.js 26.0.0 (Current)](https://nodejs.org/en/blog/release/v26.0.0) — Release notes for 26, the 2026 Current line (becomes LTS in October). 🆕 🇺🇸
- [MDN — Express Web Framework (Node.js/JavaScript) em português](https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Extensions/Server-side/Express_Nodejs) — MDN tutorial in Portuguese: from the dev environment to a complete site with Express and MongoDB.
- [Express — documentação em português](https://expressjs.com/pt-br/) — Express guide, API reference and best practices, translated.
- [npm Docs](https://docs.npmjs.com/) — Official npm docs: `package.json`, scripts, semantic versioning, publishing. 🇺🇸
- [Node.js Best Practices — versão em português](https://github.com/goldbergyoni/nodebestpractices/blob/master/README.brazilian-portuguese.md) — 100+ best practices (structure, errors, security, testing, Docker) translated by the community.
- [Node.js Best Practices (original, atualizado em 2026)](https://github.com/goldbergyoni/nodebestpractices) — The original English list, continuously maintained and reviewed. 🆕 🇺🇸
- [Alura — Node.JS: o que é, como funciona e um guia para iniciar](https://www.alura.com.br/artigos/node-js) — Portuguese article explaining the runtime and showing the first commands.
- [Alura — Arquitetura do Node.js: entenda o loop de eventos](https://www.alura.com.br/artigos/arquitetura-node-js-entenda-loop-de-eventos) — Portuguese explanation of the event loop, with diagrams.
- [Alura — Arquitetura do Node.js: conheça seus componentes](https://www.alura.com.br/artigos/arquitetura-node-js-seus-componentes) — V8, libuv, bindings and modules: how Node's pieces fit together.
- [Node.js tutorial in Visual Studio Code](https://code.visualstudio.com/docs/nodejs/nodejs-tutorial) — VS Code's official guide to creating, running and debugging Node apps. 🇺🇸

## 📚 Books
- [Livro de NodeJS (William Bruno) — código aberto](https://github.com/wbruno/livro-nodejs) — Brazilian book published in full on GitHub: fundamentals, Express, MongoDB and tests.
- [Node.js: Aplicações web real-time com Node.js (Caio Ribeiro Pereira, Casa do Código)](https://www.casadocodigo.com.br/products/livro-nodejs) — The Brazilian Node classic: asynchronous paradigm, Express and Socket.IO. 💰
- [Primeiros passos com Node.js (João Rubens, Casa do Código)](https://www.casadocodigo.com.br/products/livro-primeiros-passos-node) — From basic to intermediate: Express, middleware, authentication, MySQL, MongoDB and deployment. 💰
- [APIs Node.js (Casa do Código)](https://www.casadocodigo.com.br/products/livro-apis-nodejs) — How to build REST APIs in Node with sound structure and testing practices. 💰
- [Node.js com Express (Casa do Código)](https://www.casadocodigo.com.br/products/livro-guia-node-express) — A guide to solving and preventing common problems in Express applications. 💰
- [Coleção Node.js (Casa do Código)](https://www.casadocodigo.com.br/products/colecao-node-js) — Bundle of the publisher's Node books at a lower price. 💰
- [Aprendendo Node (Shelley Powers, Novatec)](https://novatec.com.br/livros/aprendendo-node/) — Brazilian translation of the O'Reilly book on server-side development with Node. 💰
- [Node.js Design Patterns (Casciaro e Mammino)](https://nodejsdesignpatterns.com/) — The reference on patterns, streams, architecture and scaling in Node — intermediate/advanced reading. 💰 🇺🇸
- [The definitive Node.js handbook (Flavio Copes, freeCodeCamp)](https://www.freecodecamp.org/news/the-definitive-node-js-handbook-6912378afc6e/) — Free handbook covering the essentials of Node in a single text. 🇺🇸
- [How to Get Started with NodeJS — a Handbook for Beginners (freeCodeCamp)](https://www.freecodecamp.org/news/get-started-with-nodejs/) — Newer free handbook for beginners, with hands-on examples. 🇺🇸
- [Node Hero (RisingStack)](https://blog.risingstack.com/node-hero-tutorial-getting-started-with-node-js/) — Free book-series: from your first app to testing, debugging, security and deployment. 🇺🇸
- [Eloquent JavaScript — capítulo 20: Node.js](https://eloquentjavascript.net/20_node.html) — The Node chapter of the most famous free JavaScript book. 🇺🇸
- [Eloquente JavaScript (tradução PT-BR, 4ª edição)](https://github.com/braziljs/eloquente-javascript) — Brazilian translation in progress of Eloquent JavaScript, maintained by BrazilJS.

## 🎥 YouTube channels
### In Portuguese
- [Erick Wendel](https://www.youtube.com/@ErickWendelAcademy) — Node.js core member: internals, performance, streams and platform news.
- [Rocketseat](https://www.youtube.com/@rocketseat) — Node, React and TypeScript, with frequent free events (NLW) and complete projects.
- [Matheus Battisti — Hora de Codar](https://www.youtube.com/@MatheusBattisti) — Complete free courses on Node, JavaScript, TypeScript and AI tools.
- [Filipe Deschamps](https://www.youtube.com/@FilipeDeschamps) — Fundamentals and career, with TabNews (Node.js) built in public.
- [Lucas Souza Dev](https://www.youtube.com/@LucasSouzaDev) — Complete API and front-end projects, always with Node and TypeScript.
- [Victor Lima — Guia do Programador](https://www.youtube.com/@GuiadoProgramador) — Channel with free Node.js and computer science courses.
- [balta.io](https://www.youtube.com/@baltaio) — Back-end, architecture and career, with free Node API courses.
- [Full Cycle](https://www.youtube.com/@FullCycle) — Architecture, microservices, Docker and live coding sessions with Node.js.
- [Rodrigo Branas](https://www.youtube.com/@RodrigoBranas) — Clean Code, Clean Architecture and TDD with Node/TypeScript examples.
- [Fernanda Kipper](https://www.youtube.com/@kipperdev) — Back-end, APIs and career, with hands-on projects and challenges.
- [Fabio Akita](https://www.youtube.com/@Akitando) — Long lessons on how things work underneath — runtime, operating system, history.
- [Código Fonte TV](https://www.youtube.com/@codigofontetv) — Short explanations of technologies and news, including Node, Bun and Deno.
- [Sujeito Programador](https://www.youtube.com/@Sujeitoprogramador) — Full-stack projects with Node.js, React and React Native.
- [LuizTools](https://www.youtube.com/@LuizTools) — Node.js, blockchain and career, with courses and practical tips.
- [Otávio Miranda](https://www.youtube.com/@OtavioMiranda) — Long, detailed JavaScript, TypeScript and Node courses.
- [Mario Souto — Dev Soutinho](https://www.youtube.com/@DevSoutinho) — Front-end and full stack with JavaScript, focused on career and real projects.
- [Lucas Montano](https://www.youtube.com/@LucasMontano) — Career, interviews and projects built in public.
- [CFBCursos](https://www.youtube.com/@cfbcursos) — Free, complete Node, JavaScript and database courses.

### In English
- [Node.js (canal oficial)](https://www.youtube.com/@nodejs-foundation) — Conference talks, technical meetings and project announcements. 🇺🇸
- [OpenJS Foundation](https://www.youtube.com/@OpenJSFoundation) — The foundation that hosts Node.js: OpenJS World talks and sibling projects. 🇺🇸
- [Traversy Media](https://www.youtube.com/@TraversyMedia) — Node, Express and full-stack crash courses. 🇺🇸
- [freeCodeCamp.org](https://www.youtube.com/@freecodecamp) — Complete, free multi-hour courses on Node and back-end. 🇺🇸
- [Fireship](https://www.youtube.com/@Fireship) — 100-second videos and comparisons (Node vs Bun vs Deno). 🇺🇸
- [Codevolution](https://www.youtube.com/@Codevolution) — Systematic Node and framework tutorials. 🇺🇸
- [Net Ninja](https://www.youtube.com/@NetNinja) — Short, well-edited Node, Express and MongoDB series. 🇺🇸
- [Dave Gray](https://www.youtube.com/@DaveGrayTeachesCode) — Long, complete Node and JavaScript courses. 🇺🇸
- [Programming with Mosh](https://www.youtube.com/@programmingwithmosh) — Clear introductions to Node, Express and MongoDB. 🇺🇸
- [Web Dev Simplified](https://www.youtube.com/@WebDevSimplified) — JavaScript and Node concepts explained simply. 🇺🇸
- [Hussein Nasser](https://www.youtube.com/@hnasr) — Deep back-end engineering: HTTP, TCP, databases and how Node handles connections. 🇺🇸

## 🎙️ Podcasts
- [Hipsters Ponto Tech #491 — Node.JS: O estado da arte](https://www.hipsters.tech/node-js-o-estado-da-arte-hipsters-ponto-tech-491/) — 2025 episode on Node's role in today's tooling, including the AI field. 🆕
- [Hipsters Ponto Tech #436 — Carreira Back-End e Imersão Node.js](https://www.hipsters.tech/carreira-back-end-e-imersao-node-js-hipsters-ponto-tech-436/) — How the back-end role evolved and what to study today (2024). 🆕
- [Hipsters Ponto Tech #199 — Node.js](https://www.hipsters.tech/node-js-hipsters-199/) — Modern Node and its impact on the JavaScript ecosystem.
- [Hipsters Ponto Tech — todos os episódios sobre Node.js](https://www.hipsters.tech/tag/node-js/) — Tag with every episode of Alura's podcast that discusses Node.
- [FalaDev (Rocketseat)](https://open.spotify.com/show/3TNsKUGlP9YbV1pgy3ACrW) — Rocketseat's podcast on career and development, on Spotify.
- [Syntax.fm](https://syntax.fm/) — Wes Bos and Scott Tolinski's podcast; frequent episodes on Node, Bun and Deno. 🇺🇸
- [JS Party (Changelog)](https://changelog.com/jsparty) — Weekly panel on JavaScript and the Node ecosystem. 🇺🇸

## 📰 Sites, blogs and newsletters
- [Blog oficial do Node.js](https://nodejs.org/en/blog) — Release announcements, security advisories and events — the primary source. 🆕 🇺🇸
- [Node.js Interactive 2026: A Recap](https://nodejs.org/en/blog/events/nodejs-interactive-2026) — Official recap of the 2026 event with the project's direction. 🆕 🇺🇸
- [Node Weekly](https://nodeweekly.com/) — Free weekly newsletter with the most relevant Node news and articles. 🇺🇸
- [JavaScript Weekly](https://javascriptweekly.com/) — Sister newsletter covering the whole JavaScript ecosystem. 🇺🇸
- [TabNews](https://www.tabnews.com.br/) — Brazilian technical-content community, built with Node.js and open source.
- [Blog da Rocketseat](https://www.rocketseat.com.br/blog) — Portuguese articles on Node, APIs, testing and career.
- [freeCodeCamp em português — tag Node.js](https://www.freecodecamp.org/portuguese/news/tag/node-js/) — freeCodeCamp tutorials translated into Portuguese.
- [Blog do Erick Wendel](https://blog.erickwendel.com.br/) — In-depth technical articles on Node.js and JavaScript.
- [dev.to — tag Node.js](https://dev.to/t/node) — Thousands of community articles; many in Portuguese. 🇺🇸
- [A Modern Node.js + TypeScript Setup for 2025 (Woovi, dev.to)](https://dev.to/woovi/a-modern-nodejs-typescript-setup-for-2025-nlk) — A Brazilian company's current setup: ESM, type stripping, `node --test` and no build step. 🆕 🇺🇸
- [RisingStack Engineering](https://blog.risingstack.com/) — Veteran Node blog with tutorials on performance, debugging and architecture. 🇺🇸
- [NodeSource Blog](https://nodesource.com/blog) — Articles on Node in production, security and diagnostics. 🇺🇸
- [Platformatic Blog](https://blog.platformatic.dev/) — Blog by Matteo Collina (Node TSC) and team: Fastify, performance and platform news. 🇺🇸
- [Awesome Node.js](https://github.com/sindresorhus/awesome-nodejs) — Curated list of Node packages and resources by category. 🇺🇸

## 🛠️ Tools
### Runtime, versions and packages
- [nvm](https://github.com/nvm-sh/nvm) — Node version manager for macOS/Linux: switch versions with `nvm use`. 🇺🇸
- [nvm-windows](https://github.com/nvm-windows/nvm) — The equivalent version manager for Windows. 🇺🇸
- [fnm](https://github.com/Schniz/fnm) — Fast cross-platform version manager written in Rust. 🇺🇸
- [Volta](https://volta.sh/) — Pins the Node and npm version per project automatically. 🇺🇸
- [pnpm (docs em português)](https://pnpm.io/pt/) — Fast, disk-efficient package manager, the default in monorepos. 🆕
- [Yarn](https://yarnpkg.com/) — Alternative package manager, with workspaces and plug'n'play. 🇺🇸
- [Corepack](https://github.com/nodejs/corepack#readme) — Manages the pnpm/Yarn version declared in `package.json` (`packageManager`). 🇺🇸
- [tsx](https://github.com/privatenumber/tsx) — Run TypeScript with `enum`/`namespace` and zero config when native type stripping is not enough. 🆕 🇺🇸
- [TypeScript](https://www.typescriptlang.org/) — Static types for Node; today's standard in professional projects. 🇺🇸
- [Bun](https://bun.sh/) — Ultra-fast alternative runtime, compatible with most Node APIs. 🆕 🇺🇸
- [Deno](https://deno.com/) — Secure-by-default runtime, with native TypeScript and npm compatibility. 🆕 🇺🇸
- [Imagem oficial do Node no Docker Hub](https://hub.docker.com/_/node) — `node:24-alpine`, `node:22-slim` and other tags to containerize your app. 🇺🇸
- [nodejs/docker-node — boas práticas](https://github.com/nodejs/docker-node) — The official image's repository, with a Dockerfile best-practices guide for Node. 🇺🇸

### Frameworks, databases and libraries
- [Express](https://expressjs.com/pt-br/) — Node's most used web framework; minimalist and documented in Portuguese.
- [Fastify](https://fastify.dev/) — Fast, extensible framework maintained by Node core members. 🇺🇸
- [NestJS](https://docs.nestjs.com/) — Opinionated TypeScript framework (modules, dependency injection), very common in companies. 🇺🇸
- [Hono](https://hono.dev/) — Small Web Standards-based framework; runs on Node, Bun, Deno and the edge. 🆕 🇺🇸
- [Koa](https://koajs.com/) — Minimalist framework by the creators of Express, based on `async/await`. 🇺🇸
- [AdonisJS](https://adonisjs.com/) — "Batteries-included" full-stack TypeScript framework (ORM, auth, validation). 🇺🇸
- [hapi](https://hapi.dev/) — Configuration- and security-focused framework used in large companies. 🇺🇸
- [Socket.IO](https://socket.io/) — Real-time communication (WebSocket with fallback) between a Node server and clients. 🇺🇸
- [Prisma](https://www.prisma.io/) — ORM with a fully typed client generated from the schema; great to start with. 🇺🇸
- [Drizzle ORM](https://orm.drizzle.team/) — Lightweight, TypeScript-first ORM with SQL-like syntax. 🆕 🇺🇸
- [TypeORM](https://typeorm.io/) — Decorator-based ORM, common in NestJS projects. 🇺🇸
- [Sequelize](https://sequelize.org/) — Veteran ORM for relational databases (PostgreSQL, MySQL, SQLite…). 🇺🇸
- [Knex.js](https://knexjs.org/) — SQL query builder with migrations, for people who prefer writing SQL. 🇺🇸
- [Mongoose](https://mongoosejs.com/) — ODM for MongoDB with schemas and validation. 🇺🇸
- [Zod](https://zod.dev/) — Data validation with type inference — validate `body`, `query` and environment variables. 🇺🇸
- [Undici](https://undici.nodejs.org/) — Node's official HTTP client that implements the global `fetch`. 🇺🇸
- [BullMQ](https://docs.bullmq.io/) — Background jobs and queues on top of Redis. 🇺🇸
- [Nodemailer](https://nodemailer.com/) — Sending e-mail from Node, with SMTP and providers. 🇺🇸
- [Passport.js](https://www.passportjs.org/) — Authentication with hundreds of strategies (local, OAuth, JWT). 🇺🇸
- [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken) — JWT signing and verification, the most used token library. 🇺🇸
- [Helmet](https://github.com/helmetjs/helmet) — Security HTTP headers for Express apps in one line. 🇺🇸
- [Multer](https://github.com/expressjs/multer) — File uploads (`multipart/form-data`) in Express. 🇺🇸
- [dotenv](https://github.com/motdotla/dotenv) — Loads `.env` into `process.env` (modern Node also does this with `--env-file`). 🇺🇸
- [Commander.js](https://github.com/tj/commander.js) — Build command-line tools in Node with argument parsing. 🇺🇸
- [Puppeteer](https://pptr.dev/) — Drive Chrome from Node for scraping, PDFs and automation. 🇺🇸
- [Playwright](https://playwright.dev/) — Browser automation and end-to-end testing, by Microsoft. 🇺🇸
- [json-server](https://github.com/typicode/json-server) — Fake REST API in 30 seconds from a JSON file — great for prototyping front-ends. 🇺🇸

### Testing, quality and operations
- [Vitest](https://vitest.dev/) — Fast test framework, Jest-API compatible with native TypeScript. 🆕 🇺🇸
- [Jest (docs em português)](https://jestjs.io/pt-BR/) — The most widespread test framework, with translated docs.
- [SuperTest](https://github.com/forwardemail/supertest) — Integration tests for HTTP servers with a fluent API. 🇺🇸
- [ESLint](https://eslint.org/) — The ecosystem's standard linter; catches errors before you run. 🇺🇸
- [Prettier](https://prettier.io/) — Opinionated code formatter — ends style debates. 🇺🇸
- [Biome](https://biomejs.dev/) — Linter + formatter in one tool, much faster than ESLint + Prettier. 🆕 🇺🇸
- [nodemon](https://nodemon.io/) — Restarts the app when files change (modern Node has a native `--watch`). 🇺🇸
- [PM2](https://pm2.keymetrics.io/) — Production process manager: cluster mode, auto-restart and logs. 🇺🇸
- [Pino](https://getpino.io/) — Very high-performance JSON logger, the default in Fastify. 🇺🇸
- [winston](https://github.com/winstonjs/winston) — Flexible logger with multiple transports (file, console, services). 🇺🇸
- [Clinic.js](https://clinicjs.org/) — Performance diagnostics tools (Doctor, Flame, Bubbleprof). 🇺🇸
- [autocannon](https://github.com/mcollina/autocannon) — HTTP load testing tool written in Node. 🇺🇸
- [Bruno](https://www.usebruno.com/) — Open-source API client that stores collections as Git-friendly files. 🆕 🇺🇸
- [Hoppscotch](https://hoppscotch.io/) — Open-source API client that runs in the browser. 🇺🇸
- [Insomnia](https://insomnia.rest/) — API client for REST, GraphQL and gRPC. 🇺🇸
- [Swagger / OpenAPI](https://swagger.io/) — Document and test your API with the OpenAPI specification. 🇺🇸
- [Snyk](https://snyk.io/) — Checks your `package.json` dependencies for vulnerabilities. 🇺🇸
- [Node.js Security Working Group](https://github.com/nodejs/security-wg) — The ecosystem's official security group: advisories, processes and best practices. 🇺🇸
- [Render](https://render.com/) — Hosting with a free tier to publish your Node API in minutes. 🇺🇸
- [Railway](https://railway.com/) — Simple deployment of Node apps with a database included. 🇺🇸
- [Fly.io](https://fly.io/) — Run Node containers close to users, including in São Paulo. 🇺🇸
- [Vercel](https://vercel.com/) — Serverless Node functions and full-stack app hosting. 🇺🇸
- [npm trends](https://npmtrends.com/) — Compare package downloads before picking a dependency. 🇺🇸
- [Bundlephobia](https://bundlephobia.com/) — See an npm package's size and dependencies before installing. 🇺🇸

## 🧪 Hands-on projects and challenges
- [Rinha de Backend 2025](https://github.com/zanfranceschi/rinha-de-backend-2025) — The Brazilian back-end challenge under load; hundreds of Node submissions to learn from. 🆕
- [Rinha de Backend 2024/Q1](https://github.com/zanfranceschi/rinha-de-backend-2024-q1) — Second edition: concurrency control and CPU/memory limits. 🆕
- [Rinha de Backend 2023/Q3](https://github.com/zanfranceschi/rinha-de-backend-2023-q3) — The original edition: an API under stress testing with limited resources.
- [backend-br/desafios](https://github.com/backend-br/desafios) — Brazilian collection of back-end challenges to practice and build a portfolio.
- [Backend Projects (roadmap.sh)](https://roadmap.sh/backend/projects) — Progressive projects with clear requirements, from a CLI to authenticated APIs. 🆕 🇺🇸
- [Task Tracker CLI (roadmap.sh)](https://roadmap.sh/projects/task-tracker) — Ideal first project: a task CLI using only `fs` and `process.argv`. 🆕 🇺🇸
- [learnyounode (NodeSchool)](https://github.com/workshopper/learnyounode) — Self-guided terminal workshop with 13 pure-Node exercises. 🇺🇸
- [NodeSchool](https://nodeschool.io/) — Collection of interactive Node and JavaScript workshops. 🇺🇸
- [nodejs/examples](https://github.com/nodejs/examples) — Runnable examples maintained by the Node.js project, beyond "hello world". 🇺🇸
- [Build your own X](https://github.com/codecrafters-io/build-your-own-x) — Recreate technologies from scratch (HTTP server, Redis, shell) — several Node tutorials. 🇺🇸
- [CodeCrafters](https://codecrafters.io/) — Guided challenges to build Redis, an HTTP server, Git etc. in JavaScript; partly free. 💰 🇺🇸
- [Coding Challenges (John Crickett)](https://codingchallenges.fyi/) — Weekly challenges to rebuild real tools (wc, JSON parser, load balancer). 🇺🇸
- [App Ideas](https://github.com/florinpop17/app-ideas) — Application ideas by difficulty level to practice with. 🇺🇸
- [Project-based learning](https://github.com/practical-tutorials/project-based-learning) — List of project-based tutorials, with a dedicated Node.js section. 🇺🇸
- [RealWorld](https://github.com/realworld-apps/realworld) — The "Medium clone" with dozens of Node back-end implementations to compare. 🇺🇸
- [Codewars](https://www.codewars.com/) — JavaScript katas to keep your logic sharp. 🇺🇸

## 🤖 AI in practice
Node.js and AI assistants go well together for two reasons: the ecosystem is huge (AI knows Express, Prisma and `node:test` by heart) and the runtime gives **immediate feedback** — you run the code, the test or `npm audit` and find out in seconds whether the suggestion was right. Use that to your advantage.

**For learning**
- Paste a real error (e.g. `Error [ERR_REQUIRE_ESM]`, `UnhandledPromiseRejection`, `EADDRINUSE`) together with the code snippet and ask: *"explain the cause, show the fix and tell me how to avoid it again"*.
- Ask it to **explain the event loop with a runnable example** using `setTimeout`, `setImmediate` and `process.nextTick`, run it with `node` and check that the printed order matches the explanation.
- Ask for a **guided project in steps** ("task API with Express, Zod validation and `node:test` tests") and implement each step before asking for the next.
- Ask it to **convert callback-based code to `async/await`** and then to explain what changed in error handling.
- Ask for **exercises with answer keys** on the module you are studying (`fs`, `stream`, `http`, `events`).

**For work**
- Use [GitHub Copilot](https://github.com/features/copilot), [Cursor](https://cursor.com/) or [Claude Code](https://code.claude.com/docs/en/overview) to: write integration tests with SuperTest, generate a multi-stage `Dockerfile`, migrate CommonJS → ESM, upgrade an API from Express 4 to 5, or document routes in OpenAPI.
- After **every** accepted suggestion, run `node --test` (or Vitest), the linter and `npm audit`. If the AI suggests installing a package, check on [npm trends](https://npmtrends.com/) that it exists, is maintained and has downloads — **packages invented by AI are a real attack vector** (slopsquatting).
- Prefer the built-in features the AI sometimes does not know because they are recent: `fetch` instead of axios, `node --test` instead of Jest, `--env-file` instead of dotenv, `--watch` instead of nodemon.

**Limits and good practices**
- AI **mixes versions**: it may suggest `require()` in an ESM project, removed APIs or experimental flags as if they were stable. Confirm in the [API documentation](https://nodejs.org/docs/latest/api/) for your version.
- It tends to miss a forgotten `await`, listener leaks, stream backpressure and `process.exit()` in the middle of the code. Read what you accept.
- Do not paste secrets (`.env`, tokens, connection strings), customer data or proprietary code into tools without your company's policy.
- In interviews and in production, the code is yours: understand every line.

**Node.js is the runtime of applied AI.** SDKs, agent frameworks and the Model Context Protocol have official JavaScript/TypeScript implementations that run on Node — learning Node opens the door to building products with LLMs:
- [GitHub Copilot](https://github.com/features/copilot) — AI autocomplete and chat in the editor; free for students and with a free tier. 🆕 🇺🇸
- [Cursor](https://cursor.com/) — VS Code-based editor with AI built into the workflow. 🆕 🇺🇸
- [Claude Code](https://code.claude.com/docs/en/overview) — Terminal coding agent: writes `node:test` tests, refactors and explains stack traces. 🆕 🇺🇸
- [Claude Code (playlist do Matheus Battisti)](https://www.youtube.com/playlist?list=PLnDvRpP8BnexO0yWQAf9EAbi3R_qv7D4Q) — Portuguese videos showing the agent in practice on JavaScript projects. 🆕
- [Vercel AI SDK](https://ai-sdk.dev/) — TypeScript SDK for LLM apps (streaming, tools, agents) that runs on Node. 🆕 🇺🇸
- [Anthropic TypeScript SDK](https://github.com/anthropics/anthropic-sdk-typescript) — Official SDK for using Claude models from Node. 🆕 🇺🇸
- [OpenAI Node SDK](https://github.com/openai/openai-node) — OpenAI's official JavaScript/TypeScript SDK. 🆕 🇺🇸
- [Google Gen AI SDK (js-genai)](https://github.com/googleapis/js-genai) — Official SDK for Gemini and Vertex AI in JavaScript/TypeScript. 🆕 🇺🇸
- [LangChain (JavaScript)](https://docs.langchain.com/oss/javascript/langchain/overview) — Framework for LLM, RAG and agent applications in Node. 🆕 🇺🇸
- [Mastra](https://mastra.ai/) — TypeScript framework for AI agents and workflows. 🆕 🇺🇸
- [Genkit (Google)](https://genkit.dev/) — Google's open-source framework for AI apps in JavaScript. 🆕 🇺🇸
- [LlamaIndex.TS](https://developers.llamaindex.ai/typescript/framework/) — RAG (document retrieval) framework for TypeScript/Node. 🆕 🇺🇸
- [Transformers.js (Hugging Face)](https://huggingface.co/docs/transformers.js/index) — Run AI models locally in Node (and the browser), no Python server. 🆕 🇺🇸
- [Ollama + ollama-js](https://github.com/ollama/ollama-js) — Official library to use local Ollama models (Llama, Gemma…) from Node. 🆕 🇺🇸
- [Model Context Protocol (MCP) — introdução](https://modelcontextprotocol.io/docs/2026-07-28/getting-started/intro) — The open protocol that connects AI assistants to tools and data. 🆕 🇺🇸
- [MCP — Build an MCP server](https://modelcontextprotocol.io/docs/2026-07-28/develop/build-server) — Official tutorial: write your first MCP server in Node/TypeScript. 🆕 🇺🇸
- [MCP TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk) — Official SDK for MCP servers and clients in Node. 🆕 🇺🇸
- [Claude Agent SDK (TypeScript)](https://github.com/anthropics/claude-agent-sdk-typescript) — Build agents with the same capabilities as Claude Code, in Node. 🆕 🇺🇸
- [OpenAI Agents SDK (JavaScript)](https://github.com/openai/openai-agents-js) — Lightweight framework for multi-agent workflows in Node. 🆕 🇺🇸
- [Generative AI for Beginners (Microsoft)](https://github.com/microsoft/generative-ai-for-beginners) — Free 21-lesson course, with JavaScript/Node examples. 🆕 🇺🇸

## 📜 Certifications
The OpenJS Foundation's official certifications (JSNAD and JSNSD) have been **discontinued** — the official Linux Foundation pages mark them as [inactive](https://training.linuxfoundation.org/jsnad-cert-inactive/). There is currently no official Node.js certification; employers assess **published projects and hands-on skill**. The certificates below are course-completion certificates: they help on a résumé but do not replace a portfolio.
- [Introduction to Node.js (LinuxFoundationX, edX) — certificado verificado](https://www.edx.org/learn/node-js/the-linux-foundation-introduction-to-node-js) — Linux Foundation/OpenJS course; free lessons, paid certificate. 💰 🇺🇸
- [Back End Development and APIs (freeCodeCamp) — certificação gratuita](https://www.freecodecamp.org/learn/back-end-development-and-apis) — Free certification after five Node/Express API projects. 🇺🇸
- [Curso Node JS completo (DIO) — com certificado](https://www.dio.me/curso-node-js) — Free, issues a completion certificate.
- [Curso de Node.js Grátis (Cursa) — com certificado](https://cursa.com.br/curso-de-node-js-gr%c3%a1tis/91) — Free digital certificate upon completion.
- [Formação APIs com Node.js e Express (Alura)](https://www.alura.com.br/formacao-node-js-express) — Alura certificate recognized by Brazilian companies. 💰
- [Formação Node.js (Rocketseat)](https://www.rocketseat.com.br/formacao/node) — Program completion certificate. 🆕 💰
- [Learn Node.js (Codecademy)](https://www.codecademy.com/learn/learn-node-js) — Issues a completion certificate on the Pro plan. 💰 🇺🇸

## 💼 Career and jobs
Node.js is a requirement in most JavaScript back-end and full-stack job posts in Brazil, almost always alongside TypeScript, a framework (Express, NestJS or Fastify), a database (PostgreSQL or MongoDB) and Docker. Tip: in the GitHub job repositories below, search open issues for "Node".
- [Stack Overflow Developer Survey 2025](https://survey.stackoverflow.co/2025/) — Node.js remains among the most used technologies by professionals worldwide. 🆕 🇺🇸
- [State of JavaScript 2024](https://2024.stateofjs.com/en-US/) — Annual ecosystem survey: runtimes, frameworks, trends and salaries. 🆕 🇺🇸
- [backend-br/vagas](https://github.com/backend-br/vagas) — Back-end jobs in Brazil posted as issues; search for "Node".
- [Programathor — vagas Node.js](https://programathor.com.br/jobs-node-js) — Tech jobs in Brazil filtered by Node.js.
- [GeekHunter](https://www.geekhunter.com/pt) — Brazilian platform where companies make offers to developers.
- [Coodesh](https://coodesh.com/) — Tech jobs in Brazil with standardized hiring processes.
- [Remotar](https://remotar.com.br/) — 100% remote jobs for Brazilians.
- [RemoteOK — vagas Node.js](https://remoteok.com/remote-node-jobs) — International remote Node jobs. 🇺🇸
- [Node.js Basics — perguntas de entrevista (learning-zone)](https://github.com/learning-zone/nodejs-basics) — Hundreds of Node interview questions and answers, updated for v24. 🆕 🇺🇸
- [Tech Interview Handbook](https://www.techinterviewhandbook.org/) — Complete preparation for technical interviews. 🇺🇸

## 👥 Communities
- [Discord oficial do Node.js](https://discord.com/invite/nodejs) — The project's official server, launched in 2025, with help and announcement channels. 🆕 🇺🇸
- [Anúncio do Discord oficial (blog do Node.js)](https://nodejs.org/en/blog/announcements/official-discord-launch-announcement) — Official post explaining the partnership with the Nodeiflux community. 🆕 🇺🇸
- [GitHub Discussions do Node.js](https://github.com/orgs/nodejs/discussions) — Questions and discussions directly with the project team. 🇺🇸
- [nodejs/help](https://github.com/nodejs/help) — Official repository to ask for help with Node.js. 🇺🇸
- [Como contribuir com o Node.js](https://nodejs.org/en/about/get-involved) — Official "Get involved" page: working groups, mentoring and first steps. 🇺🇸
- [Guia de pull requests do Node.js](https://github.com/nodejs/node/blob/main/doc/contributing/pull-requests.md) — How to send your first PR to Node core. 🇺🇸
- [NodeBR (Telegram)](https://t.me/nodebr) — Brazilian Node.js group on Telegram.
- [NodeBR (GitHub)](https://github.com/nodebr) — The NodeBR community organization with materials and projects.
- [Back-End Brasil](https://github.com/backend-br) — Brazilian back-end community: jobs, challenges and forum.
- [BrazilJS](https://www.braziljs.org/) — Community and newsletter of Brazil's largest JavaScript conference.
- [Rocketseat (Discord)](https://discord.com/invite/rocketseat) — One of Brazil's largest developer communities, with Node channels.
- [TabNews](https://www.tabnews.com.br/) — Brazilian technical-content community created by Filipe Deschamps.
- [He4rt Developers](https://heartdevs.com/) — Brazilian open-source community with an active Discord and Node/TypeScript projects.
- [Desenvolvedores Brasil (Discord)](https://discord.com/invite/t3vYGUuK6P) — Brazilian community with tips, courses, mentoring and job posts.
- [Lista de grupos de tecnologia no Telegram (TI-Brasil)](https://github.com/TI-Brasil/lista-telegram-brasil) — Directory of Brazilian Telegram groups, including Node.js and JavaScript.
- [DEV Community — devs brasileiros](https://dev.to/t/braziliandevs) — Tag with Portuguese articles from the Brazilian community.
- [r/node](https://www.reddit.com/r/node/) — The Node.js community subreddit. 🇺🇸
- [OpenJS Foundation](https://openjsf.org/) — Foundation that hosts Node.js, Express, Fastify, Mocha and other projects. 🇺🇸
- [Node Congress](https://nodecongress.com/) — Annual online conference dedicated to Node.js. 🇺🇸

## 🚨 How to contribute
Found a broken link, a new course or a tool that deserves to be here? Open an issue using the repository templates or send a pull request. Criteria: working link, legal content that is free or clearly marked as paid, with a one-line description. Details in [CONTRIBUTING.md](../CONTRIBUTING.md).

## 📄 License
This project is under the [MIT](../LICENSE) license. Made with 💙 by [Arthur Coutinho (@arthurspk)](https://github.com/arthurspk) and the [Guia Dev Brasil](https://github.com/arthurspk/guiadevbrasil) community.

## 💙 Support the project
Star this repository and the [main guide](https://github.com/arthurspk/guiadevbrasil), share it with someone who is starting out and follow the project on social media:

[<img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">](https://github.com/arthurspk)
[<img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">](https://www.linkedin.com/in/arthurspk/)
[<img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" alt="X (Twitter)">](https://x.com/manotoquinho)
[<img src="https://img.shields.io/badge/instagram-%23E4405F.svg?&style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram">](https://www.instagram.com/arthurspk/)
[<img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook">](https://www.facebook.com/seixasqlc/)
