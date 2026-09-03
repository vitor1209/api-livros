# 📚 API de Livros

### Sistemas Web II · 3º Bimestre · Etec MCM

**Uma aplicação completa para gerenciamento de livros, desenvolvida do banco de dados ao Front End.**

[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](https://www.python.org/) [![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/) [![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)](https://www.mysql.com/) [![XAMPP](https://img.shields.io/badge/XAMPP-FB7A24?logo=apache&logoColor=white)](https://www.apachefriends.org/) [![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML) [![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/docs/Web/CSS) [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=111111)](https://developer.mozilla.org/docs/Web/JavaScript)
---

## 🎯 Sobre o projeto

Este projeto foi desenvolvido como **trabalho avaliativo do 3º Bimestre da disciplina de Sistemas Web II (SW-II)** da **Etec Professora Maria Cristina Medeiros (Etec MCM)**.

A proposta é construir uma aplicação web completa para gerenciamento de livros, utilizando uma **API REST com FastAPI**, banco de dados **MySQL** e uma interface desenvolvida com **HTML, CSS e JavaScript**.

O projeto foi pensado para acompanhar todo o fluxo de uma aplicação web:

```text
Banco de Dados
      ↓
   FastAPI
      ↓
     CRUD
      ↓
  Front End
      ↓
  Navegador
```

👨‍💻 **Desenvolvido por Vitor Lopes**

---

## 📖 Funcionalidades

A aplicação terá um CRUD completo de livros.

| 🟢 Operação | Método   | Descrição                      |
| ----------- | -------- | ------------------------------ |
| Create      | `POST`   | Cadastrar um novo livro        |
| Read        | `GET`    | Listar e consultar livros      |
| Update      | `PUT`    | Atualizar os dados de um livro |
| Delete      | `DELETE` | Excluir um livro               |

Cada livro possui os seguintes dados:

| Campo            | Tipo     | Descrição                         |
| ---------------- | -------- | --------------------------------- |
| `id`             | Inteiro  | Identificador único               |
| `titulo`         | Texto    | Título do livro                   |
| `autor`          | Texto    | Autor do livro                    |
| `ano_publicacao` | Inteiro  | Ano de publicação                 |
| `disponivel`     | Booleano | Indica se o livro está disponível |

---

## 🧠 Organização do projeto

A aplicação será dividida em duas partes principais.

### ⚙️ Backend

Responsável pela API, regras da aplicação, validação dos dados e comunicação com o banco MySQL.

Tecnologias utilizadas:

* 🐍 Python
* ⚡ FastAPI
* 🗄️ MySQL
* 🔗 SQLAlchemy
* 🐬 PyMySQL
* 🚀 Uvicorn
* 🧪 Pydantic

### 🎨 Front End

Responsável pela interface utilizada pelo usuário para consumir a API.

Tecnologias utilizadas:

* 🌐 HTML
* 🎨 CSS
* ⚡ JavaScript
* 🔄 `fetch`

---

## 🗂️ Estrutura do projeto

```text
api-livros/
│
├── backend/
│   ├── main.py
│   ├── database.py
│   ├── models.py
│   ├── schemas.py
│   └── rotas/
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── database/
│   └── biblioteca_db.sql
│
├── .env
├── .gitignore
├── requirements.txt
└── README.md
```

> A estrutura pode evoluir ao longo das aulas conforme novas partes da aplicação forem implementadas.

---

## 🧩 Projeto desenvolvido em 4 aulas

O desenvolvimento da aplicação será realizado **gradualmente durante quatro aulas**, seguindo uma sequência de implementação.

A ideia é construir o projeto por etapas, entendendo cada parte antes de avançar para a próxima.

### 🟦 Aula 01 · Fundação FastAPI + MySQL

📄 [01-fundacao-fastapi-mysql.md](https://github.com/ProfAndersonVanin/nova_api/blob/main/01-fundacao-fastapi-mysql.md)

Nesta etapa será realizada a configuração inicial do projeto:

* criação do ambiente Python;
* instalação das dependências;
* configuração do FastAPI;
* configuração do MySQL;
* utilização do XAMPP;
* criação do banco `biblioteca_db`;
* configuração do `phpMyAdmin`;
* conexão da aplicação com o banco;
* criação de uma rota inicial para testar a API.

### 🟩 Aula 02 · Modelo + POST + GET

📄 [02-modelo-post-get.md](https://github.com/ProfAndersonVanin/nova_api/blob/main/02-modelo-post-get.md)

Nesta etapa será construída a estrutura principal dos livros:

* criação do modelo `Livro`;
* criação dos schemas;
* configuração da sessão do banco;
* criação da rota `POST`;
* criação da rota `GET`;
* cadastro de livros;
* listagem dos livros;
* validação dos dados.

### 🟧 Aula 03 · PUT + DELETE + CRUD

📄 [03-put-delete-crud.md](https://github.com/ProfAndersonVanin/nova_api/blob/main/03-put-delete-crud.md)

Nesta etapa o CRUD será finalizado:

* implementação do `PUT`;
* implementação do `DELETE`;
* atualização de livros;
* exclusão de livros;
* tratamento de erros HTTP;
* validação das operações;
* testes do CRUD completo.

### 🟥 Aula 04 · Front End HTML + CSS + JavaScript

📄 [04-frontend-html-css-js.md](https://github.com/ProfAndersonVanin/nova_api/blob/main/04-frontend-html-css-js.md)

Na última etapa será construída a interface web:

* criação da página HTML;
* estilização com CSS;
* criação da lógica em JavaScript;
* consumo da API com `fetch`;
* listagem dos livros;
* cadastro de livros;
* edição de livros;
* exclusão de livros;
* integração completa entre Front End e Backend.

---

## 🛠️ Stack utilizada

| Tecnologia    | Utilização                       |
| ------------- | -------------------------------- |
| 🐍 Python     | Linguagem principal do Backend   |
| ⚡ FastAPI     | Construção da API REST           |
| 🗄️ MySQL     | Banco de dados                   |
| 🧰 XAMPP      | Ambiente local para Apache/MySQL |
| 🐘 phpMyAdmin | Administração do banco           |
| 🔗 SQLAlchemy | ORM e acesso ao banco            |
| 🚀 Uvicorn    | Servidor da aplicação            |
| 🌐 HTML       | Estrutura do Front End           |
| 🎨 CSS        | Estilização da interface         |
| ⚡ JavaScript  | Lógica e consumo da API          |
| 💻 VS Code    | Ambiente de desenvolvimento      |
| 🐙 Git/GitHub | Versionamento                    |

---

## 📐 Padrão de código

Uma das propostas do projeto é manter o código **simples, legível e didático**.

Por isso, nomes de classes, funções e variáveis próprias serão escritos preferencialmente em **português**.

### ✅ Exemplos

```python
class Livro:
    ...
```

```python
def criar_livro():
    ...
```

```python
def listar_livros():
    ...
```

```python
def atualizar_livro():
    ...
```

```python
def excluir_livro():
    ...
```

Também serão utilizados nomes como:

```text
Livro
LivroCriacao
LivroResposta
resultado
consulta
livro
livros
```

A ideia é manter a lógica fácil de acompanhar e preservar a consistência entre Backend e Front End.

---

## 🗃️ Banco de dados

O projeto utiliza o banco:

```text
biblioteca_db
```

O banco será executado localmente utilizando o **MySQL do XAMPP** e administrado pelo **phpMyAdmin**.

O arquivo SQL permanecerá versionado no repositório:

```text
database/biblioteca_db.sql
```

Assim, o banco pode ser recriado sempre que necessário.

> 🔒 O arquivo `.env` não deve ser enviado ao GitHub, pois pode conter informações de configuração e credenciais locais do banco.

---

## 🚀 Como executar o projeto

### 1️⃣ Clonar o repositório

```bash
git clone https://github.com/SEU_USUARIO/api-livros.git
cd api-livros
```

### 2️⃣ Criar o ambiente virtual

```bash
python -m venv venv
```

### 3️⃣ Ativar o ambiente virtual

No Windows:

```bash
venv\Scripts\activate
```

### 4️⃣ Instalar as dependências

```bash
pip install -r requirements.txt
```

### 5️⃣ Iniciar o XAMPP

No XAMPP, iniciar:

```text
Apache
MySQL
```

Depois, acessar o `phpMyAdmin` e importar:

```text
database/biblioteca_db.sql
```

### 6️⃣ Configurar o `.env`

Criar o arquivo:

```text
.env
```

E adicionar as configurações necessárias para conexão com o banco.

### 7️⃣ Executar a API

```bash
uvicorn main:app --reload
```

A documentação automática do FastAPI estará disponível em:

```text
http://127.0.0.1:8000/docs
```

---

## 🔌 Endpoints

Ao final do projeto, a API terá operações semelhantes a:

| Método   | Endpoint       | Função             |
| -------- | -------------- | ------------------ |
| `GET`    | `/livros`      | Listar livros      |
| `GET`    | `/livros/{id}` | Consultar um livro |
| `POST`   | `/livros`      | Criar livro        |
| `PUT`    | `/livros/{id}` | Atualizar livro    |
| `DELETE` | `/livros/{id}` | Excluir livro      |

> Os endpoints podem sofrer pequenos ajustes durante o desenvolvimento das aulas.

---

## 🧪 Fluxo da aplicação

O Front End consumirá diretamente a API através de requisições HTTP.

```text
┌─────────────────────┐
│      Front End      │
│  HTML + CSS + JS    │
└──────────┬──────────┘
           │
           │ fetch()
           ▼
┌─────────────────────┐
│       FastAPI       │
│      API REST       │
└──────────┬──────────┘
           │
           │ SQLAlchemy
           ▼
┌─────────────────────┐
│        MySQL        │
│    biblioteca_db    │
└─────────────────────┘
```

---

## 📅 Cronograma

| Etapa | Conteúdo                 | Data       |
| ----- | ------------------------ | ---------- |
| 🟦 01 | Fundação FastAPI + MySQL | 02/09/2026 |
| 🟩 02 | Modelo + POST + GET      | 09/09/2026 |
| 🟧 03 | PUT + DELETE + CRUD      | 16/09/2026 |
| 🟥 04 | Front End                | 23/09/2026 |

---

## ✅ Objetivos do projeto

Ao finalizar o projeto, será possível:

* ✅ criar uma API utilizando FastAPI;
* ✅ trabalhar com `GET`, `POST`, `PUT` e `DELETE`;
* ✅ conectar Python a um banco MySQL;
* ✅ utilizar XAMPP e phpMyAdmin;
* ✅ criar models e schemas;
* ✅ validar dados;
* ✅ tratar erros HTTP;
* ✅ construir uma interface com HTML e CSS;
* ✅ utilizar JavaScript para consumir uma API;
* ✅ utilizar `fetch`;
* ✅ trabalhar com Git e GitHub;
* ✅ desenvolver uma aplicação completa do Backend ao Front End.

---

## 📚 Material das aulas

Todo o desenvolvimento está separado em quatro arquivos:

1. 📘 [01-fundacao-fastapi-mysql.md](https://github.com/ProfAndersonVanin/nova_api/blob/main/01-fundacao-fastapi-mysql.md)
2. 📗 [02-modelo-post-get.md](https://github.com/ProfAndersonVanin/nova_api/blob/main/02-modelo-post-get.md)
3. 📙 [03-put-delete-crud.md](https://github.com/ProfAndersonVanin/nova_api/blob/main/03-put-delete-crud.md)
4. 📕 [04-frontend-html-css-js.md](https://github.com/ProfAndersonVanin/nova_api/blob/main/04-frontend-html-css-js.md)

Cada arquivo representa uma aula e uma etapa da construção da aplicação.

---

## 👨‍💻 Autor

### Vitor Lopes

🎓 Etec Professora Maria Cristina Medeiros
💻 Desenvolvimento Web · Python · FastAPI · JavaScript
📚 Projeto de Sistemas Web II · 3º Bimestre

---

### 📚 Do banco de dados ao navegador.

**Projeto desenvolvido por Vitor Lopes · Etec MCM · 2026**
