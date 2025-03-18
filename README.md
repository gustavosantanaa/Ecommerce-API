# 🚀 Ecommerce API 

Este projeto é uma API REST simples para gerenciar usuários utilizando **Node.js, Express e Firebase Firestore**.

## 📌 Funcionalidades
- Listar todos os usuários
- Obter um usuário por ID
- Criar um novo usuário
- Atualizar um usuário existente
- Excluir um usuário

---

## 🛠️ Tecnologias Utilizadas
- **Node.js**
- **Express** (Framework para criação de APIs)
- **Firebase Firestore** (Banco de dados NoSQL)
- **TypeScript** (Tipagem estática)

---

## 🔧 Requisitos
Antes de rodar o projeto, certifique-se de ter instalado:
- **Node.js** (versão 14 ou superior)
- **Firebase CLI** (caso precise autenticar o Firestore)

Instale as dependências com:
```sh
npm install
```

---

## 🚀 Como Usar

### 1️⃣ Clone o repositório:
```sh
git clone https://github.com/seuusuario/Ecommerce-API.git
cd Ecommerce-API
```

### 2️⃣ Configure o Firebase
Você precisa configurar o Firebase Admin SDK com as credenciais do seu projeto. Crie um arquivo `.env` e adicione:
```sh
FIREBASE_CREDENTIALS=./caminho/para/seu/arquivo.json
```

Certifique-se de inicializar o Firebase no seu código.

### 3️⃣ Execute o servidor:
```sh
npm run dev
```

A API estará disponível em **http://localhost:3000**

---

## 📡 Endpoints da API

### 🔍 **Listar todos os usuários**
```http
GET /users
```
**Resposta:**
```json
[
  {
    "id": "1",
    "nome": "João Silva",
    "email": "joao@email.com"
  }
]
```

### 🔍 **Buscar um usuário por ID**
```http
GET /users/:id
```

### ➕ **Criar um usuário**
```http
POST /users
```
**Body:**
```json
{
  "nome": "Maria Souza",
  "email": "maria@email.com"
}
```

### ✏️ **Atualizar um usuário**
```http
PUT /users/:id
```
**Body:**
```json
{
  "nome": "Maria Souza",
  "email": "maria@email.com"
}
```

### ❌ **Excluir um usuário**
```http
DELETE /users/:id
```

---

## 🤝 Contribuição
Sinta-se à vontade para contribuir! Para isso:
1. Faça um **fork** do projeto
2. Crie uma **branch** para sua feature (`git checkout -b minha-feature`)
3. Faça um **commit** das suas mudanças (`git commit -m 'Adicionando nova feature'`)
4. Envie para o repositório (`git push origin minha-feature`)
5. Crie um **Pull Request**

