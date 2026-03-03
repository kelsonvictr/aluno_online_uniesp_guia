# 📚 Aluno Online — Guia Interativo de Backend

> Tutorial interativo e ultra-didático para a disciplina de **Backend com Java/Spring Boot** da **UNIESP** — João Pessoa, PB.

<p align="center">
  <img src="https://img.shields.io/badge/Java-17-f89820?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring%20Boot-3.4-6db33f?style=for-the-badge&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Deploy-Vercel-000?style=for-the-badge&logo=vercel&logoColor=white" />
</p>

---

## 🎯 Sobre

Este é um **guia interativo em HTML** (single-page) que acompanha os alunos na construção passo a passo da API REST **Aluno Online** — do primeiro `@Entity` ao histórico acadêmico completo com DTOs.

O material foi criado para alunos em **primeiro contato com programação backend**, explicando cada conceito, anotação e camada com analogias do mundo real, diagramas animados e simulações interativas.

🔗 **Acesse o guia:** [aluno-online-uniesp-guia.vercel.app](https://aluno-online-uniesp-guia.vercel.app)

🔗 **Repositório do projeto ensinado:** [kelsonvictr/aluno_online_2025_1](https://github.com/kelsonvictr/aluno_online_2025_1)

---

## 📖 Conteúdo

O tutorial é dividido em **5 capítulos**, organizados na ordem em que são ensinados em aula:

| # | Capítulo | Tópicos |
|---|---------|---------|
| 1 | **👨‍🎓 CRUD de Aluno** | Model, Repository, Service, Controller — CRUD completo |
| 2 | **👨‍🏫 Professor** | Reforço do padrão MVC com segunda entidade |
| 3 | **📖 Disciplina** | `@ManyToOne`, Foreign Key, Derived Queries |
| 4 | **📝 Matrícula** | Enum, regras de negócio, `@PatchMapping`, cálculo de média |
| 5 | **📦 DTOs** | Request/Response DTOs, histórico acadêmico |

### Seções introdutórias

- Visão geral do projeto e stack tecnológico
- Arquitetura em camadas (Controller → Service → Repository → DB)
- Setup do projeto (Spring Initializr + `application.properties`)
- Estrutura de pacotes

---

## ✨ Elementos Interativos

| Elemento | Descrição |
|----------|-----------|
| 🔄 **Fluxo animado** | Animação passo a passo do caminho request → controller → service → repo → DB |
| 💻 **Terminal simulado** | Simulação de requests/responses no estilo Swagger/Insomnia |
| 🗄️ **Banco interativo** | Tabela de banco de dados que cresce conforme o aluno clica em "inserir" |
| 🏷️ **Tooltips de anotações** | Hover sobre `@Entity`, `@Autowired`, `@ManyToOne` etc. para ver explicações |
| 📖 **Togglers** | Seções expansíveis "O que cada anotação faz?", "O que é Optional?" etc. |
| 📊 **Barra de progresso** | Indicador de leitura no topo da página |
| 📚 **Menu lateral** | Sumário navegável com todos os capítulos e seções |

---

## 🚀 Deploy

O projeto é um **único arquivo HTML** (sem dependências), feito para deploy simples na Vercel:

```bash
# O deploy é automático via integração com GitHub
# Basta fazer push para a branch main
git push origin main
```

### Deploy manual (Vercel CLI)

```bash
npm i -g vercel
vercel --prod
```

---

## 🏗️ Estrutura

```
.
├── index.html    ← Tutorial interativo completo (single-file)
└── README.md     ← Este arquivo
```

> **Por que um único arquivo?** Para facilitar o deploy na Vercel e permitir que os alunos abram localmente sem nenhuma configuração — basta dar duplo-clique no `index.html`.

---

## 🛠️ Stack do Guia

- **HTML5** — Estrutura semântica
- **CSS3** — Design dark mode, animações, responsivo
- **JavaScript** — Interatividade (demos, togglers, fluxo animado)
- **Google Fonts** — JetBrains Mono, Nunito, Caveat

### Stack ensinada no guia

- **Java 17**
- **Spring Boot 3.4.3** (Web, Data JPA)
- **PostgreSQL**
- **Lombok**
- **Swagger/OpenAPI** (springdoc)

---

## 👨‍🏫 Metodologia

A abordagem pedagógica segue esta ordem deliberada:

1. **Model direto primeiro** — Os alunos aprendem usando a entidade JPA diretamente nos controllers, sem DTOs, para entender o fluxo completo sem abstrações extras.

2. **CRUD simples → complexo** — Começa com Aluno (CRUD básico), depois Professor (reforço), Disciplina (introduz relacionamentos) e Matrícula (regras de negócio).

3. **DTOs por último** — Só depois que os alunos dominam o fluxo Model → Repo → Service → Controller é que DTOs são introduzidos, com a justificativa clara de "por que não usar o Model direto?".

4. **Analogias em tudo** — Cada conceito técnico tem uma analogia do mundo real (Repository = funcionário do arquivo, Service = gerente, API = garçom, etc.).

---

## 📄 Licença

Material didático de uso livre para fins educacionais.

Feito com 💜 para os alunos da **UNIESP** — João Pessoa, PB.
