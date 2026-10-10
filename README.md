# DDD031

 English version below | 🇧🇷 [Clique aqui para a versão em Português](#português)

🔗 **Live demo / Demo ao vivo:** https://ddd031.onrender.com
👤 **Demo login / Login de demonstração:** `demo` / `demo123`

> ⏳ Free hosting tier (Render): first load after inactivity may take up to ~1 minute.
> Hospedagem gratuita (Render): o primeiro acesso após inatividade pode levar até ~1 minuto.

---

## English

### About

DDD031 helps young people (18–30) discover places to go out in Belo Horizonte, Brazil —
cafés, bars, restaurants, parks, and cultural spots — without needing to search across
multiple sources. The focus is on accessible venues that don't require advance ticket
purchases, making spontaneous discovery easy.

Beyond listing places, the platform encourages interaction: users can favorite venues,
discuss them in a forum, vote as a group on where to go ("Match"), or let a random pick
decide ("Roulette").

This repository is an individual, portfolio-oriented adaptation of a group academic
project built for a first-semester Interdisciplinary Work course at PUC Minas (Brazil).

### Original team

| Name | Role |
|---|---|
| Alex de Castro Mendes Marques | UX/UI Design |
| Júlia Michetti Costa Santos | Back-end Development |
| **Matheus Akl Barbalho Falqueto** | **Front-end Development (me)** |

**Faculty advisors:** Rommel Vieira Carneiro, Bernardo Guerra Pereira Cunha, Walisson Ferreira de Carvalho.

### My contribution

As the front-end developer, I was responsible for:
- The **Favorites** feature (UI and logic)
- The **Discoveries** section (home highlights)
- **Random Place / Roulette**
- **FAQ**
- **Match** (group voting system)

### Features

- 🏠 **Home:** featured places, search by name/category, tag filters
- ❤️ **Favorites:** save preferred venues (per user)
- 🗨️ **Forum:** create threads and replies, filter by category and tags
- 🎲 **Roulette:** randomly picks a place
- 🤝 **Match:** group voting system to decide on a place
- 💑 **Dates:** section dedicated to date spots
- ❓ **FAQ:** 18 frequently asked questions
- 🗺️ **Map:** general view of Belo Horizonte
- 👥 **About Us:** team presentation

### Tech stack

- **Back-end:** Node.js, Express, [json-server](https://github.com/typicode/json-server) (REST API)
- **Front-end:** Vanilla JavaScript, HTML, CSS
- **Maps:** Leaflet + OpenStreetMap
- **Hosting:** Render

### Project structure

```
├── server.js          # Express + json-server
├── db/db.json          # Database (places, users, forum, FAQ)
└── public/              # Front-end
    ├── index.html, favorites.html, forum.html, match.html, roulette.html...
    └── assets/
        ├── js/          # Page logic
        ├── css/          # Styles
        └── images/       # Images and avatars
```

### Run locally

```bash
git clone https://github.com/Akl372/ddd031.git
cd ddd031
npm install
npm start
```
Visit `http://localhost:3000`.

### Known limitations

- The forum ships with sample threads for demo purposes; new posts don't persist
  permanently, since the free hosting tier has no persistent database between restarts.
- The map currently shows Belo Horizonte generally, without individual markers for the
  21 listed places — a planned improvement for a future version.

### License

Academic project under the CC-BY-4.0 license, following the original group repository.

---

## Português

### Sobre o projeto

O DDD031 é uma plataforma web que ajuda jovens de 18 a 30 anos a descobrir onde sair em
Belo Horizonte — cafés, bares, restaurantes, parques e pontos culturais — sem precisar
pesquisar em múltiplos lugares. O foco é em locais acessíveis, que não exigem compra
antecipada de ingresso, facilitando descobertas espontâneas.

Além de listar lugares, o site promove interação entre os usuários: eles podem favoritar
locais, discutir no fórum, decidir onde ir em grupo através de uma votação (Match), ou
deixar a sorte escolher (Roleta).

Este repositório é uma adaptação individual, com fins de portfólio, de um projeto
acadêmico desenvolvido em trio para a disciplina de Trabalho Interdisciplinar (1º período)
da PUC Minas.

### Equipe original

| Nome | Função |
|---|---|
| Alex de Castro Mendes Marques | Design UX/UI |
| Júlia Michetti Costa Santos | Desenvolvimento Back-end |
| **Matheus Akl Barbalho Falqueto** | **Desenvolvimento Front-end (eu)** |

**Professores responsáveis:** Rommel Vieira Carneiro, Bernardo Guerra Pereira Cunha, Walisson Ferreira de Carvalho.

### Minha contribuição

Como desenvolvedor front-end do projeto, fui responsável por:
- Funcionalidade de **Favoritos** (interface e lógica)
- Seção **Descobertas** (destaques da home)
- **Lugar Aleatório / Roleta**
- **FAQ**
- **Match** (sistema de votação em grupo)

### Funcionalidades

- 🏠 **Home:** lugares em destaque, busca por nome/categoria, filtros por tag
- ❤️ **Favoritos:** salvar locais preferidos (por usuário)
- 🗨️ **Fórum:** criação de tópicos e respostas, filtro por categoria e tags
- 🎲 **Roleta:** sorteia um local aleatoriamente
- 🤝 **Match:** sistema de votação para decidir um lugar em grupo
- 💑 **Dates:** seção dedicada a locais para encontros
- ❓ **FAQ:** 18 perguntas frequentes
- 🗺️ **Mapa:** visualização geral de Belo Horizonte
- 👥 **Sobre Nós:** apresentação da equipe

### Tecnologias

- **Back-end:** Node.js, Express, [json-server](https://github.com/typicode/json-server) (API REST)
- **Front-end:** JavaScript puro (sem framework), HTML, CSS
- **Mapas:** Leaflet + OpenStreetMap
- **Hospedagem:** Render

### Como rodar localmente

```bash
git clone https://github.com/Akl372/ddd031.git
cd ddd031
npm install
npm start
```
Acesse `http://localhost:3000`.

### Limitações conhecidas

- O fórum vem com tópicos de exemplo para demonstração; novos posts não persistem
  permanentemente, já que o plano gratuito de hospedagem não mantém um banco de dados
  persistente entre reinícios.
- O mapa mostra Belo Horizonte de forma geral, sem marcar individualmente os 21 locais
  cadastrados — melhoria planejada para uma próxima versão.

### Licença

Projeto acadêmico sob licença CC-BY-4.0, conforme o repositório original do grupo.
