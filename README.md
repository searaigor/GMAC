# 🏥 GMAC - Gerenciamento de Medicamentos de Alto Custo

Sistema backend desenvolvido para gerenciamento de pacientes, validação de documentação e controle de concessão de medicamentos de alto custo, com suporte a agendamento de perícias médicas e geração de relatórios estratégicos.

---

## 🚀 Objetivo do Projeto

O **GMAC** foi desenvolvido com o objetivo de simular um sistema real utilizado por instituições de saúde para:

* Gerenciar o cadastro de pacientes
* Validar documentações obrigatórias
* Determinar elegibilidade para medicamentos de alto custo
* Agendar perícias médicas quando necessário
* Permitir avaliação médica presencial
* Gerar dashboards com dados estratégicos

Este projeto foi construído com foco em **boas práticas de backend, segurança e arquitetura**, simulando um ambiente próximo ao mercado.

---

## 🧠 Principais Skills Demonstradas

* 🔐 **Autenticação e autorização com JWT**
* 🛡️ **Controle de acesso baseado em roles (Spring Security)**
* 🧱 **Arquitetura em camadas (Controller → Service → Repository)**
* 🗃️ **Modelagem de dados com JPA / Hibernate**
* 🐘 **Integração com PostgreSQL**
* 🔄 **Versionamento de banco com Flyway**
* ⚙️ **Configuração via variáveis de ambiente (.env)**
* 📊 **Construção de endpoints**
* 🧪 **Boas práticas de organização e separação de responsabilidades**

---

## 🏗️ Arquitetura

O projeto segue uma arquitetura em camadas:

* **Controller** → Responsável pelas requisições HTTP
* **Service** → Regras de negócio
* **Repository** → Acesso ao banco de dados
* **Security** → Configuração de autenticação e autorização (JWT)

---

## 🔐 Controle de Acesso

O sistema utiliza controle de acesso baseado em perfis:

* `ADMINISTRADOR`
* `RECEPCIONISTA`
* `MEDICO`

Cada endpoint possui restrições específicas conforme o perfil do usuário.

---

## 📌 Principais Funcionalidades

### 👤 Usuários

* Cadastro e gerenciamento de usuários do sistema
* Controle de permissões por role

### 🧑‍⚕️ Pacientes

* Cadastro completo de pacientes
* Associação de endereço e documentos
* Consulta e atualização de dados

### 📄 Documentação

* Validação de documentos
* Consulta por ID e status
* Controle de elegibilidade

### 🩺 Perícia Médica

* Agendamento de perícia
* Validação por médico
* Cancelamento e remarcação

### 📊 Relatórios

* Dashboard com dados estratégicos para tomada de decisão

---

## 🛠️ Tecnologias Utilizadas

* **Java 17+**
* **Spring Boot**
* **Spring Security**
* **JWT (JSON Web Token)**
* **Spring Data JPA / Hibernate**
* **PostgreSQL**
* **Flyway**
* **Maven**

---


## 🔑 Autenticação

A autenticação é feita via JWT:

* Endpoint: `POST /auth/login`
* Retorna um token que deve ser enviado no header:

```http
Authorization: Bearer {token}
```

---

## 📌 Endpoints

A API está organizada por módulos:

* 🔐 Autenticação
* 👤 Usuários
* 🧑‍⚕️ Pacientes
* 📄 Documentação
* 🩺 Perícia
* 📊 Relatórios

> Consulte a documentação completa dos endpoints no projeto.

---

## 💼 Contexto de Desenvolvimento

Este projeto foi desenvolvido com foco em evolução como desenvolvedor backend, aplicando conceitos fundamentais utilizados no mercado, como:

* Segurança com Spring Security
* Arquitetura limpa e organizada
* Separação de responsabilidades
* Boas práticas com APIs REST

---

## 📈 Possíveis Melhorias Futuras

* Adição de testes automatizados
* Containerização com Docker
* Integração com Swagger/OpenAPI
* Implementação de cache (Redis)
* Observabilidade (logs e métricas)

---

* 💼 Focado em desenvolvimento backend com Java e Spring Boot

---
