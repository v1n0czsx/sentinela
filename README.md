# 🏥 Sistema Hospitalar Web

Sistema desenvolvido para simular o fluxo de atendimento de um hospital, permitindo login de usuários e cadastro de pacientes para triagem.

## 🚀 Funcionalidades

- 🔐 Login de usuários
- 👨‍⚕️ Cadastro de pacientes
- 📋 Registro de CPF
- 🏥 Seleção do tipo de atendimento
- 🔄 Integração com API REST
- 🎨 Interface responsiva

## 🛠️ Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript
- Fetch API
- Node.js
- Express.js

## 📁 Estrutura do Projeto

```bash
Sistema-Hospitalar/
│
├── index.html
├── atendimento.html
├── style.css
└── backend/
```

## 🔑 Sistema de Login

O sistema realiza autenticação através da API e redireciona automaticamente o usuário para sua área correspondente:

- Atendimento
- Triagem
- Médico

## 👨‍⚕️ Cadastro de Pacientes

Permite registrar:

- Nome
- CPF
- Tipo de atendimento
  - Convênio
  - Particular

Os dados são enviados para a API utilizando requisições HTTP.

## 📡 Endpoints

### Login

```http
POST /login
```

Exemplo:

```json
{
  "usuario": "admin",
  "senha": "123456"
}
```

### Atendimento

```http
POST /atendimento
```

Exemplo:

```json
{
  "nome": "João Silva",
  "cpf": "123.456.789-00",
  "tipo": "Convenio"
}
```

## ▶️ Como Executar

Clone o projeto:

```bash
git clone https://github.com/SEU-USUARIO/sistema-hospitalar.git
```

Entre na pasta:

```bash
cd sistema-hospitalar
```

Inicie o backend:

```bash
npm install
npm start
```

Abra o arquivo:

```bash
index.html
```

## 📷 Fluxo do Sistema

```text
Login
  ↓
Atendimento
  ↓
Triagem
  ↓
Médico
```

