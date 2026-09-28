# API RESTful - Alunos e Cursos

Este repositório contém, por agora, as Partes 1 e 2 da Atividade Prática #1:

## Parte 1: Base de Dados (JSON)

Ficheiro [mock-data/bd.json](mock-data/bd.json) com:

- `alunos`: `id`, `nome`, `apelido`, `idCurso`, `anoCurricular`
- `cursos`: `id`, `nomeDoCurso`

## Parte 2: API Simulada com JSON-Server

### Como correr

```bash
cd mock-server
npm install
npm start
```

O servidor arranca em `http://localhost:3001` e expõe:

- `GET /alunos` — listar alunos
- `GET /alunos/:id` — obter um aluno
- `POST /alunos` — criar aluno
- `PUT /alunos/:id` / `PATCH /alunos/:id` — atualizar aluno
- `DELETE /alunos/:id` — apagar aluno
- `GET /cursos` — listar cursos
- `GET /cursos/:id` — obter um curso

### Testes Postman

Coleção exportada em [tests/postman_collection.json](tests/postman_collection.json), com pedidos CRUD para `alunos` e leitura de `cursos`. Importar no Postman e definir a variável `baseUrl` (default `http://localhost:3001`).
