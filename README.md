# 🛠️ Complexo - Backend

API REST desenvolvida em **Spring Boot** para gerenciar estúdios de tatuagem, artistas, agendamentos e perfis públicos. Este backend dá suporte à aplicação frontend - https://github.com/jeffmqs/complexo-frontend.git

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)

---

## 📌 Visão Geral

Este projeto oferece as funcionalidades do backend para a plataforma Complexo, incluindo:

- Autenticação com JWT
- Cadastro de estúdios e artistas
- Upload de imagens (galeria e perfil)
- Agendamentos
- Páginas públicas de estúdios
- API REST para consumo do frontend

---

## 🗃️ Estrutura da API

- `/auth/login` → Login com validação e JWT
- `/usuarios` → CRUD de estúdios
- `/usuarios/{id}` → Visualizar, atualizar ou deletar um estúdio
- `/agendamentos` → Criar e listar agendamentos
- `/artistas` → Adicionar artistas vinculados a estúdios

---

## 🔐 Segurança

- Implementação de autenticação com Spring Security
- Proteção de rotas privadas com JWT
- CORS configurado para permitir comunicação com o frontend (Vite/React)

---

## 💾 Banco de Dados

- PostgreSQL (local e remoto)
- Suporte a múltiplas conexões: local, ElephantSQL, Render, NeonDB

---

## ⚙️ Como rodar o projeto

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/complexo-backend.git

# Importe o projeto em sua IDE (IntelliJ, Eclipse ou VSCode)

# Configure o arquivo application.properties:
spring.datasource.url=jdbc:postgresql://localhost:5432/complexo
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha

# Rode a aplicação (Spring Boot App)
