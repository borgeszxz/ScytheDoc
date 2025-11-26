# Scythe

Bem-vindo à **Scythe**, uma plataforma completa de e-commerce desenvolvida para a venda e gerenciamento de softwares digitais. Este projeto foi construído com foco em **segurança**, **design moderno** (estilo Cyberpunk/Glassmorphism) e **experiência do usuário**.

A plataforma oferece um ecossistema robusto que conecta os usuários finais aos seus produtos através de um dashboard intuitivo e fornece aos administradores controle total sobre vendas e licenças.

## 📸 Imagens do Projeto

![Home](https://i.imgur.com/A3aNQoY.png)
![Home](https://i.imgur.com/t05Up4k.png)
![Home](https://i.imgur.com/szonBBN.png)
![Store](https://i.imgur.com/9tRGhSm.png)
![Store](https://i.imgur.com/P3nUbYi.png)
![Status](https://i.imgur.com/vuthxKd.png)
![Dashboard](https://i.imgur.com/dmviJys.png)
![Dashboard](https://i.imgur.com/pP3xFKU.png)
![Dashboard](https://i.imgur.com/89zJWJr.png)

## 🚀 Tecnologias Utilizadas

O projeto foi desenvolvido utilizando uma arquitetura moderna, separando claramente o Frontend e o Backend para garantir escalabilidade e manutenção.

### 🎨 Frontend (Client & Admin)
*   **Vue.js 3 (Composition API):** Framework progressivo para construção de interfaces reativas e modulares.
*   **Vite:** Build tool de próxima geração para desenvolvimento rápido e otimizado.
*   **Tailwind CSS:** Framework CSS utilitário para estilização rápida e consistente.
*   **Design System:** Implementação de **Glassmorphism** e estética "Dark/Cyberpunk" com animações suaves.
*   **Vue Router:** Gerenciamento de rotas e navegação (SPA).

### ⚙️ Backend (API REST)
*   **Node.js & Express:** Servidor robusto e flexível para gerenciar as requisições da API.
*   **MySQL:** Banco de dados relacional para armazenamento seguro de usuários, produtos e logs.
*   **JWT (JSON Web Tokens):** Sistema de autenticação seguro e stateless.
*   **Bcrypt.js:** Hashing de senhas para garantir a segurança dos dados dos usuários.
*   **Multer:** Gerenciamento de upload de imagens para os produtos da loja.

### 🔐 Integrações & Segurança
*   **KeyAuth API:** Integração direta com o sistema de licenciamento KeyAuth para validação, ativação e reset de HWID de chaves de software.
*   **Proteção de Rotas:** Middleware de autenticação para proteger endpoints sensíveis (Admin/User).
*   **Validação de Licenças:** Sistema inteligente que verifica o status da licença (Ativa, Expirada, Banida) antes de permitir o download do software.

---

## ✨ Funcionalidades Principais

### 👤 Área do Cliente (Dashboard)
*   **Registro e Login Seguro:** Conta de usuário protegida com JWT.
*   **Ativação de Chaves:** O usuário pode ativar suas licenças KeyAuth diretamente pelo site, vinculando-as à sua conta Scythe.
*   **Gestão de Assinaturas:** Visualização clara do tempo restante, status da licença e produto associado.
*   **Download Protegido:** O download do loader só é liberado se o usuário possuir uma licença **Ativa** e o produto estiver com status **Undetected**.
*   **Reset HWID:** Sistema automatizado para resetar o HWID da licença (com cooldown de 24h) em caso de troca de PC.

### 🛡️ Painel Administrativo
*   **Gestão de Produtos:** CRUD completo (Criar, Ler, Atualizar, Deletar) para os produtos da loja.
    *   Upload de imagens.
    *   Definição de preços, status (Undetected/Detected/Updating) e funcionalidades.
*   **Controle de Usuários:** Visualização de todos os usuários com licenças ativas.
*   **Sistema de Banimento:**
    *   **Banir Key:** Invalida uma licença específica.
    *   **Banir Usuário:** Bloqueia permanentemente o acesso de um usuário ao sistema.
    *   **Unban:** Reverte as ações de banimento.

---

## 📂 Estrutura do Projeto

O projeto é organizado em duas partes principais:

*   **Backend:** API REST desenvolvida em Node.js/Express com integração MySQL e KeyAuth.
*   **Frontend:** Interface moderna desenvolvida em Vue.js 3 com design Glassmorphism e sistema de rotas SPA.

---

Desenvolvido por **Borges**.

---

# Scythe

Welcome to **Scythe**, a complete e-commerce platform developed for selling and managing premium digital software. This project was built with a focus on **security**, **modern design** (Cyberpunk/Glassmorphism style), and **user experience**.

The platform offers a robust ecosystem that connects end users to their products through an intuitive dashboard and provides administrators with complete control over sales and licenses.

## 📸 Project Images

![Home](https://i.imgur.com/A3aNQoY.png)
![Home](https://i.imgur.com/t05Up4k.png)
![Home](https://i.imgur.com/szonBBN.png)
![Store](https://i.imgur.com/9tRGhSm.png)
![Store](https://i.imgur.com/P3nUbYi.png)
![Status](https://i.imgur.com/vuthxKd.png)
![Dashboard](https://i.imgur.com/dmviJys.png)
![Dashboard](https://i.imgur.com/pP3xFKU.png)
![Dashboard](https://i.imgur.com/89zJWJr.png)

## 🚀 Technologies Used

The project was developed using a modern architecture, clearly separating Frontend and Backend to ensure scalability and maintainability.

### 🎨 Frontend (Client & Admin)
*   **Vue.js 3 (Composition API):** Progressive framework for building reactive and modular interfaces.
*   **Vite:** Next-generation build tool for fast and optimized development.
*   **Tailwind CSS:** Utility-first CSS framework for rapid and consistent styling.
*   **Design System:** Implementation of **Glassmorphism** and "Dark/Cyberpunk" aesthetic with smooth animations.
*   **Vue Router:** Route management and navigation (SPA).

### ⚙️ Backend (REST API)
*   **Node.js & Express:** Robust and flexible server to manage API requests.
*   **MySQL:** Relational database for secure storage of users, products, and logs.
*   **JWT (JSON Web Tokens):** Secure and stateless authentication system.
*   **Bcrypt.js:** Password hashing to ensure user data security.
*   **Multer:** Image upload management for store products.

### 🔐 Integrations & Security
*   **KeyAuth API:** Direct integration with the KeyAuth licensing system for validation, activation, and HWID reset of software keys.
*   **Route Protection:** Authentication middleware to protect sensitive endpoints (Admin/User).
*   **License Validation:** Intelligent system that checks license status (Active, Expired, Banned) before allowing software download.

---

## ✨ Main Features

### 👤 Client Area (Dashboard)
*   **Secure Registration and Login:** User account protected with JWT.
*   **Key Activation:** Users can activate their KeyAuth licenses directly through the site, linking them to their Scythe account.
*   **Subscription Management:** Clear visualization of remaining time, license status, and associated product.
*   **Protected Download:** The loader download is only released if the user has an **Active** license and the product status is **Undetected**.
*   **HWID Reset:** Automated system to reset license HWID (with 24h cooldown) in case of PC change.

### 🛡️ Administrative Panel
*   **Product Management:** Complete CRUD (Create, Read, Update, Delete) for store products.
    *   Image upload.
    *   Price definition, status (Undetected/Detected/Updating), and features.
*   **User Control:** View all users with active licenses.
*   **Ban System:**
    *   **Ban Key:** Invalidates a specific license.
    *   **Ban User:** Permanently blocks a user's access to the system.
    *   **Unban:** Reverses ban actions.

---

## 📂 Project Structure

The project is organized into two main parts:

*   **Backend:** REST API developed in Node.js/Express with MySQL and KeyAuth integration.
*   **Frontend:** Modern interface developed in Vue.js 3 with Glassmorphism design and SPA routing system.

---

Developed by **Borges**.
