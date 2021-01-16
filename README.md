# Digital Innovation One

## Desenvolvimento de testes unitários para validar uma API REST de gerenciamento de estoques de cerveja

Esse exercício ensinou a testar, unitariamente, uma API REST para o gerenciamento de estoques de cerveja. Os testes unitários foram construídos para validar o nosso sistema de gerenciamento de estoques de cerveja, desenvolvido em **Spring Boot**, além de apresentar os principais conceitos e vantagens de criar testes unitários com **JUnit** e **Mockito**.
As funcionalidades da REST API foram construídas através da prática do **TDD** (*Test Driven Development*).

````console
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 21, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  01:02 min
[INFO] Finished at: 2021-01-15T23:41:32-03:00
[INFO] ------------------------------------------------------------------------

Process finished with exit code 0
````

---

### 📑 Instruções

Para executar o projeto são necessários os seguintes pré-requisitos:

- Java 14 ou versões superiores.
- Maven 3.6.3 ou versões superiores.

Para executar o projeto, digite o seguinte comando na raiz do projeto:

```console
mvn spring-boot:run
```

Para executar a suíte de testes, digite o seguinte comando:

```console
mvn clean test
```

Para acessar a REST API, utilize o seguinte *endpoint*:

```console
http://localhost:8080/api/v1/beers
```

---

### ⚙ REST API

| Endpoint: | Method: | Descrição: | Response Status Code: |
|-----------|---------|--------------|-----------------------|
| /beers | GET  | Retorna uma lista com todas as cervejas. | 200 |
| /beers/{id} | GET | Retorna uma cerveja específica. | 200 / 404 |
| /beers | POST | Cria uma nova entidade Beer no sistema. | 201 / 400 / 404 |
| /beers/{id} | DELETE | Deleta uma cerveja específica. | 204 / 404 |
| /beers/{id}/increment | PATCH | Modifica a quantidade de uma cerveja específica.| 200 / 400 / 404 |

---

### 📚 Referências

- [Java SE Development Kit 15 Download](https://www.oracle.com/java/technologies/javase-jdk15-downloads.html)
- [Maven](https://maven.apache.org/)
- [Insomnia](https://insomnia.rest/download/)

- [Spring Boot](https://spring.io/projects/spring-boot)

- [Site oficial JUnit 5](https://junit.org/junit5/docs/current/user-guide/)
- [Site oficial Mockito](https://site.mockito.org/)
- [Site oficial Hamcrest](http://hamcrest.org/JavaHamcrest/)

- [Documentação oficial do Lombok](https://projectlombok.org/)
- [Documentação oficial do Map Struct](https://mapstruct.org/)
- [Referência para o padrão arquitetural REST](https://restfulapi.net/)
