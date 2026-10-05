# 🚀 Node.js + Fastify CRUD API

API REST desenvolvida com **Node.js** e **Fastify**, criada para demonstrar operações CRUD de forma simples, rápida e organizada.

O projeto permite **criar, consultar, atualizar e excluir itens** através de endpoints HTTP.

## 🛠️ Tecnologias

- Node.js
- Fastify
- JavaScript
- API REST
- JSON
- NPM

## 📁 Estrutura do Projeto

```text
NODE-FASTIFY-CRUD-API/
├── data.js
├── routes.js
├── server.js
├── package.json
└── README.md
```

### Principais arquivos

**`server.js`**  
Responsável por iniciar o servidor Fastify na porta `3000`.

**`routes.js`**  
Contém as rotas da API e as operações CRUD.

**`data.js`**  
Responsável pelo armazenamento e gerenciamento dos itens em memória.

**`package.json`**  
Contém as configurações do projeto, scripts e dependências.

## ⚙️ Instalação

Clone o repositório:

```bash
git clone https://github.com/seu-usuario/NODE-FASTIFY-CRUD-API.git
```

Entre na pasta:

```bash
cd NODE-FASTIFY-CRUD-API
```

Instale as dependências:

```bash
npm install
```

## ▶️ Executando o projeto

Inicie a API com:

```bash
npm run dev
```

O servidor será executado em:

```text
http://localhost:3000
```

## 📡 Endpoints

| Método | Endpoint | Descrição |
|---|---|---|
| GET | `/items` | Lista todos os itens |
| GET | `/items/:id` | Busca um item pelo ID |
| POST | `/items` | Cria um novo item |
| PUT | `/items/:id` | Atualiza um item |
| DELETE | `/items/:id` | Remove um item |

## 📝 Exemplos

### Listar itens

```http
GET /items
```

Resposta:

```json
[
  {
    "id": "123456789",
    "name": "Produto 1",
    "price": 100
  }
]
```

### Criar item

```http
POST /items
```

Body:

```json
{
  "name": "Produto 1",
  "price": 100
}
```

### Buscar item

```http
GET /items/123456789
```

### Atualizar item

```http
PUT /items/123456789
```

Body:

```json
{
  "name": "Produto atualizado",
  "price": 150
}
```

### Excluir item

```http
DELETE /items/123456789
```

Resposta:

```json
{
  "success": true
}
```

## 💾 Armazenamento

Atualmente, os dados são armazenados **em memória**, através do arquivo `data.js`.

Isso significa que os dados são perdidos quando o servidor é encerrado ou reiniciado.

## 🔮 Melhorias futuras

- Integração com PostgreSQL
- Validação de dados e schemas
- Documentação com Swagger/OpenAPI
- Tratamento de erros mais completo
- Variáveis de ambiente com `.env`
- Testes automatizados
- Autenticação e autorização
- Dockerização da aplicação

## 🎯 Objetivo

O projeto foi desenvolvido como prática de **desenvolvimento de APIs REST**, utilizando Node.js e Fastify, com foco na implementação dos principais conceitos de um CRUD.

## 👨‍💻 Autor

**Matheus Barcelli**

Desenvolvedor em formação e estudante de Engenharia de Software.

### Tecnologias e interesses

- 💻 Desenvolvimento de Software
- 🌐 APIs REST
- 🟢 Node.js
- ⚡ Fastify
- ☕ Java
- 🗄️ Banco de Dados
- 🐧 Linux
- 🔧 Git & GitHub

---

⭐ Se este projeto foi útil para você, considere deixar uma estrela no repositório!
