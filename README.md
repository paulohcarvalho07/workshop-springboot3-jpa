# Workshop Spring Boot 3 com JPA

[![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.5.3-green)](https://spring.io/projects/spring-boot)
[![Java](https://img.shields.io/badge/Java-17-orange)](https://openjdk.org/projects/jdk/17/)

---

## 📖 Descrição

📌 Este projeto é uma iniciativa educacional que explora o uso do Spring Boot 3 em conjunto com JPA para criar um sistema de gerenciamento de pedidos e produtos. Durante o workshop, foram abordados conceitos essenciais como entidades, repositórios, controladores REST, perfis de execução, manipulação de datas, relacionamentos entre entidades e tratamento de exceções.

---

## 🎯 Objetivo

O objetivo principal é desenvolver uma aplicação completa utilizando:

* Configuração de entidades JPA com relacionamentos
* Repositórios Spring Data com consultas personalizadas
* Camada de serviço e controladores REST
* Validações e tratamento de exceções
* Boas práticas de estruturação de projetos Spring

---

## ⚙️ Funcionalidades

* Gerenciamento de pedidos e produtos através de entidades e repositórios JPA
* Utilização de diferentes perfis de execução para ambientes de desenvolvimento e produção
* Manipulação de datas e timestamps para rastreamento de criação e atualização
* Implementação de relacionamentos entre entidades, como pedidos e produtos
* Tratamento de exceções personalizado através de Exception Handling

---

## 🏗 Arquitetura / Estrutura do Projeto

```plaintext
src/
├── main/
│   ├── java/com/example/demo/
│   │   ├── entities/
│   │   │   ├── Pedido.java
│   │   │   ├── Produto.java
│   │   │   └── ...
│   │   ├── repositories/
│   │   │   ├── PedidoRepository.java
│   │   │   ├── ProdutoRepository.java
│   │   │   └── ...
│   │   ├── services/
│   │   │   ├── PedidoService.java
│   │   │   ├── ProdutoService.java
│   │   │   └── ...
│   │   ├── controllers/
│   │   │   ├── PedidoController.java
│   │   │   ├── ProdutoController.java
│   │   │   └── ...
│   │   ├── exceptions/
│   │   │   └── ResourceNotFoundException.java
│   │   └── DemoApplication.java
│   └── resources/
│       ├── application.properties
│       └── import.sql
└── test/
    └── java/com/example/demo/
```

* **entities/**: Classes de domínio com anotações JPA
* **repositories/**: Interfaces Spring Data JPA
* **services/**: Lógica de negócio e regras de aplicação
* **controllers/**: Endpoints REST da aplicação
* **exceptions/**: Tratamento personalizado de exceções

---

## 🛠 Tecnologias

* **Spring Boot**: 3.5.3 (framework principal)
* **Java 17**: Linguagem de programação
* **Spring Data JPA**: Persistência de dados
* **H2 Database**: Banco de dados em memória
* **Maven**: Gerenciamento de dependências
* **Hibernate**: Implementação JPA

---

## 🔧 Pré-requisitos

* JDK 17 instalado
* Maven 3.6+
* IDE com suporte a Spring (IntelliJ, Eclipse ou VS Code)
* Postman ou similar para testar endpoints

---

## 🖥 Uso

1. **Clonar e importar o projeto**

   ```bash
   git clone https://github.com/paulohcarvalho07/workshop-springboot3-jpa
   cd workshop-springboot3-jpa
   ```

2. **Executar a aplicação**

   ```bash
   ./mvnw spring-boot:run
   ```

3. **Acessar endpoints**

   ```http
   GET http://localhost:8080/pedidos
   GET http://localhost:8080/produtos
   POST http://localhost:8080/pedidos
   ```

4. **Acessar H2 Console**

   ```http
   URL: http://localhost:8080/h2-console
   JDBC URL: jdbc:h2:mem:testdb
   Username: sa
   Password: (vazio)
   ```

5. **Testar operações CRUD**

   * Use Postman para testar todos os endpoints
   * Consulte os controllers para ver os métodos disponíveis
   * Dados iniciais são carregados automaticamente via `import.sql`

---

## 📬 Contato

* **Autor**: Paulo Carvalho
* **GitHub**: [paulohcarvalho07](https://github.com/paulohcarvalho07)
