# Ecoleta
[README (en-us)](README-en-us.md)

Aplicação web 
## Requisitos

- [NodeJS 12.*](https://nodejs.org/en/download/)
- [Kotlin 1.3.72](https://sdkman.io/)

## Tecnologias/Frameworks

- [Spring Boot](https://spring.io/projects/spring-boot)
- [Undertow](http://undertow.io/)
- [Swagger](https://swagger.io/)
- [Jackson](https://github.com/FasterXML/jackson)
- [Flyway](https://flywaydb.org/)
- [Postgres](https://www.postgresql.org/)
- [H2](http://www.h2database.com/html/main.html)
- [Logback](https://logback.qos.ch/)
- [OpenTracing](https://opentracing.io/)
- [ktlint](https://ktlint.github.io/)
- [JaCoCo](https://www.eclemma.org/jacoco/)
- [Kotest](https://github.com/kotest/kotest)
- [MockK](https://mockk.io/)
- [Gradle](https://gradle.org/)

## Padrões de projeto

- *Clean Architecture*

## Execução

Para executar a aplicação, basta executar a task *bootRun* do Gradle Wrapper.

```shell script
./gradlew bootRun
```

Caso possua um ambiente *docker* configurado, execute o seguinte arquivo:

```shell script
./build.sh
```
Obs: Para mais informações de *build*, utilize a *flag* `--help` no *script*.

## Endpoints

- URL: http://localhost:8080/
- Swagger: http://localhost:8080/swagger-ui.html
- Info: http://localhost:8080/info
- Health: http://localhost:8080/health
    
## Como colaborar

- ### *Branch*
    O nosso ciclo de desenvolvimento se inicia na *branch* **alpha**, onde todos os nossos testes de novas *features*
    são testados, em seguida, a **alpha** é *mergeada* na **beta**, onde estará apenas as *features* que irão para
    produção no próximo *release*, por fim, a **master** conterá apenas as *features* vigentes em produção.

- ### *Commit*
    Antes efetuar qualquer *commit*, sempre verifique quais arquivos você criou, alterou ou removeu.
    ```shell script
    git status
    ```
    Caso contenha algum arquivo ou diretório que não seja propriamente código, favor adicioná-lo no [.gitignore](.gitignore).
    
    Antes de ser feito um commit, sempre deverá ser executado o [ktlint](https://ktlint.github.io/).
    
    ```shell script
    ./gradlew ktlintFormat
    ```
  
- ### *Pull Request*
    Antes de abrir um *pull request*, conferir se todas as suas modificações foram sincronizadas com a *branch* que será *mergeada*.
    
    Marque o seu *user* na *flag 'Assignees'* e escolha a *label* que melhor se adeque ao seu *pull request*.
