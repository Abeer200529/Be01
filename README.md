# Tiny Backend (BE-01) — Spring Boot

A minimal Spring Boot app with two JSON endpoints.

## Prerequisites

- Java 17+ installed (`java -version` to check)
- Maven installed (`mvn -version` to check) — or use the Maven wrapper if your IDE generates one

## Run

```
mvn spring-boot:run
```

Server starts at http://localhost:8081

(First run will take a minute — Maven downloads Spring Boot dependencies.)

## Endpoints

- `GET /health` → `{"status":"ok"}`
- `GET /hello` → `{"message":"Hello, world!"}`

## Test with curl

```
curl http://localhost:8080/health
curl http://localhost:8080/hello
```

## Test in browser

Open http://localhost:8081/health or http://localhost:8081/hello directly in your browser.

## Project structure

```
be01/
├── pom.xml
└── src/main/java/com/flyrank/be01/
    ├── Be01Application.java   (entry point)
    |__ controller
      └── HelloController.java   (the two endpoints)
```

## Publish to GitHub

```
git init
git add .
git commit -m "BE-01: minimal backend with two JSON endpoints"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

Make sure the repository is set to **Public** so reviewers can access the link.
