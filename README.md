# Buildium Real Estate Management System

Buildium is a real estate management monorepo with a Spring Boot API, Oracle Database persistence, and separate Angular dashboards for administrators and clients.

## Features

- Java Spring Boot backend for property, client, transaction, and administrative workflows
- Oracle Database integration through JPA and the Oracle JDBC driver
- Swagger/OpenAPI support for backend API exploration
- Angular admin dashboard for managing real estate operations and records
- Angular client portal for browsing properties and managing client-facing workflows
- Bootstrap-based responsive interface styling across both frontends
- Maven-based backend build and npm-based frontend development workflow

## Tech Stack

| Layer | Technology |
| --- | --- |
| Backend | Java 8, Spring Boot, Spring Data JPA, Maven |
| Database | Oracle Database, Oracle JDBC |
| Admin Frontend | Angular 6, Bootstrap, ngx-bootstrap |
| Client Frontend | Angular 6, Bootstrap, ng-bootstrap |
| API Docs | Springfox Swagger |

## Project Structure

```text
.
|-- Buildium API Manager/   Spring Boot backend API
|-- Buildium Admin App/     Angular administrator dashboard
|-- Buildium Client App/    Angular client portal
|-- Run Mannual.txt         Original local run notes
`-- README.md
```

## Prerequisites

| Tool | Version |
| --- | --- |
| Java | 8 |
| Maven | 3.x |
| Node.js | 10.x to 12.x recommended for Angular 6 |
| Angular CLI | 6.1.x |
| Oracle Database | 11g/12c compatible |

## Backend Setup

```bash
cd "Buildium API Manager"
mvn clean install
mvn spring-boot:run
```

Configure Oracle connection settings in the backend application properties before starting the API.

## Admin Dashboard

```bash
cd "Buildium Admin App"
npm install
npm start
```

Default Angular URL:

```text
http://localhost:4200
```

## Client Portal

```bash
cd "Buildium Client App"
npm install
npm start
```

If both Angular apps are running together, start one on a different port:

```bash
ng serve --port 4300
```

## Notes

This project targets an older Angular and Java stack. Use the documented versions above for the smoothest local setup.
