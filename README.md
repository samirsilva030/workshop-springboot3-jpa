# Sobre o projeto

O Workshop Spring Boot 3 + JPA é uma aplicação backend construída para estudo dos principais recursos do ecossistema Spring, com foco em:

Estruturação de um projeto em camadas
Mapeamento objeto-relacional com JPA / Hibernate
Relacionamentos entre entidades
Criação de web services REST
Tratamento de exceções
Execução de um banco de dados H2 em memória
Seed automático de dados usando CommandLineRunner

Esse projeto simula uma plataforma simples de e-commerce, contendo:

Usuários
Pedidos
Produtos
Categorias
Itens do pedido
Pagamento do pedido

## Modelo conceitual
A aplicação segue o seguinte modelo:

User → 1:N → Order
Order → 1:1 → Payment
Product ↔ N:N ↔ Category
Order ↔ N:N (com atributos) ↔ Product via OrderItem
OrderItem possui a chave composta OrderItemPK

# Tecnologias utilizadas
- Back end
- Java 17
- Spring Boot 3
- Spring Web
- Spring Data JPA
- Hibernate
- Banco H2
- Maven

# Como executar o projeto

## Back end
- Java 17
- Maven

```bash
# clonar repositório
git clone https://github.com/samirsilva030/workshop-springboot3-jpa

# entrar na pasta
cd workshop-springboot3-jpa

# executar o projeto
./mvnw spring-boot:run
```

# Autor
Samir Silva Furtado

https:www.linkedin.com/in/samir-silva-16abb7265
