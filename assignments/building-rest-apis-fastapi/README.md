# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objetivo

Construa uma API REST para gerenciar um catálogo de livros usando FastAPI. Você praticará métodos HTTP, validação de dados, códigos de status e documentação automática, mantendo os dados em memória.

## 📝 Tarefas

### 🛠️ Criar a aplicação e consultar livros

#### Descrição
Crie uma aplicação FastAPI para um catálogo de livros. Comece com alguns livros de exemplo armazenados em uma lista e disponibilize uma rota para consultar o catálogo.

#### Requisitos
O programa concluído deve:

- Criar uma aplicação FastAPI que possa ser iniciada com Uvicorn
- Representar cada livro com `id`, `title` e `author`
- Implementar `GET /books` para retornar a lista de livros
- Permitir consultar a documentação interativa em `/docs`


### 🛠️ Adicionar e consultar um livro

#### Descrição
Permita que clientes adicionem livros ao catálogo e consultem um livro individual pelo seu identificador. Use um modelo Pydantic para validar os dados enviados.

#### Requisitos
O programa concluído deve:

- Implementar `POST /books` para criar um livro com título e autor obrigatórios
- Gerar um identificador único para cada livro criado
- Retornar o livro criado com o código de status HTTP `201 Created`
- Implementar `GET /books/{book_id}` e retornar `404 Not Found` quando o livro não existir


### 🛠️ Atualizar e remover livros

#### Descrição
Complete as operações de gerenciamento do catálogo implementando rotas para atualizar e remover livros existentes.

#### Requisitos
O programa concluído deve:

- Implementar `PUT /books/{book_id}` para atualizar o título e o autor de um livro
- Implementar `DELETE /books/{book_id}` para remover um livro existente
- Retornar `404 Not Found` para atualizações ou remoções de identificadores inexistentes
- Usar códigos de status adequados para operações concluídas e confirmar os resultados pelas rotas de consulta
