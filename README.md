# CRUD PHP + JavaScript

Projeto utilizado para estudo de **requisições HTTP, APIs e operações CRUD**, utilizando JavaScript no frontend e PHP no backend.

Este repositório é baseado no projeto e tutorial **PHP and JS HTTP CRUD**, criado por [Victor Raphael](https://github.com/victor-raphael17/php-and-js-http-crud). O código original foi utilizado como material de estudo, com algumas adaptações no ambiente Docker.

## Tecnologias

* PHP 8.3
* JavaScript
* HTML e CSS
* Bootstrap
* Axios
* Vite
* Docker
* Docker Compose
* Apache

## Funcionalidades

A aplicação realiza as operações básicas de um CRUD de usuários:

* `GET` — listar usuários;
* `POST` — cadastrar usuário;
* `PUT` — atualizar usuário;
* `PATCH` — atualizar parcialmente;
* `DELETE` — remover usuário.

O frontend realiza requisições HTTP para a API PHP, que processa as operações e persiste os dados em JSON.

```text
Frontend → Axios → API PHP → Dados JSON
```

## Estrutura

```text
crud-CodeAcademy/
├── api/
│   ├── config/
│   ├── data/
│   ├── public/
│   ├── src/
│   └── Dockerfile
├── frontend/
│   ├── src/
│   ├── Dockerfile
│   └── package.json
└── compose.yaml
```

## Executando

Com Docker e Docker Compose instalados:

```bash
git clone https://github.com/lucasbrugge/crud-CodeAcademy.git
cd crud-CodeAcademy
docker compose up --build
```

Acesse:

* **Frontend:** `http://localhost:8080`
* **API:** `http://localhost:8000/api/users`

Para encerrar:

```bash
docker compose down
```

## Créditos

Projeto original e material de estudo desenvolvido por **Victor Raphael**:

* [Tutorial PHP and JS HTTP CRUD](https://victor-raphael17.github.io/php-and-js-http-crud/http-crud-tutorial.html)
* [Repositório original](https://github.com/victor-raphael17/php-and-js-http-crud)

Este repositório foi utilizado para **estudo, reprodução do projeto e compreensão de sua arquitetura e funcionamento**, com adaptações no ambiente de execução.
