# First Spring Boot App – Spring MVC with Thymeleaf (Exercise 16, Task 1)

My first Spring Boot web application: a Spring controller that returns plain text with `@ResponseBody` and an HTML page (view) built with Thymeleaf, following the MVC pattern.
Exercise 16 – *First two Spring Framework apps*, Akademia Finansów i Biznesu Vistula.

## Technologies

- Java 21
- Spring Boot 4 (Spring Web, Thymeleaf, Lombok)
- Maven
- Project generated with Spring Initializr (https://start.spring.io)

## How to run

1. Open the project in IntelliJ IDEA.
2. Wait for Maven to download the dependencies.
3. Run `FirstProjectJavaSpringApplication`.
4. The application starts on `http://localhost:8080`.

## Endpoints

| URL | What it returns |
| --- | --- |
| http://localhost:8080 | Plain text: *Hello Vistula, in my first Spring controller.* |
| http://localhost:8080/greeting | HTML page: *Hello, World!*, a text and the Vistula logo |
| http://localhost:8080/greeting?name=Vistula | HTML page: *Hello, Vistula!*, a text and the Vistula logo |

## How it works

- `HelloController` is marked with `@Controller`. In a `@Controller`, the `String` a method returns is treated as the **name of a
