# Lojinha API Automação
Esse repositório contém a automação de alguns testes de API Rest de um software denominado Lojinha. Seguem algumas decisões tomadas na estruturação do projeto.

## Tecnologias Utilizadas
- Java
  https://www.oracle.com/br/java/technologies/javase-jdk16-downloads.html
- RestAssured
  https://mvnrepository.com/artifact/io.rest-assured/rest-assured/4.4.0
- JUnit
  https://mvnrepository.com/artifact/org.junit/junit-bom/5.7.1
- Maven
  https://maven.apache.org/


## Testes Automatizados
- Testes para validar as partições de equivalência relacionadas ao valor do produto da Lojinha, no qual, segundo as regras de negócio, menciona que o valor do produto deve estar entre R$ 0,01 e R$7.000,00.


## Notas Gerais

- Sempre utilizamos a notação *beforeEach* para capturar o Token que será utilizado posteriormente nos métodos de teste.
- Armazenamos os dados que são enviados para a API através do uso das classes POJO.
- Criamos dados iniciais através do uso da classe Data Factory, para facilitar a criação e controle dos mesmos.
- Por utilizar o JUnit 5 nesse projeto, foi possível utilizar a anotação *DisplayName* para gerar descrições em Português para nossos testes.    