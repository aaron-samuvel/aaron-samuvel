# Hi, I'm Aaron 👋

### Java Developer | Spring Boot | Spring MVC | Apache Tomcat

I build maintainable Java web applications with clear MVC boundaries, secure deployment, and performance designed around measured workloads.

## Java stack

- **Backend:** Java, Spring Boot, Spring MVC, REST APIs
- **Web views:** JSP, JSTL, Jakarta Servlet, JSP tag libraries
- **Runtime:** Apache Tomcat, XML deployment descriptors, Tomcat server.xml, executable WARs
- **Data:** PostgreSQL, Spring Data JPA, Flyway migrations
- **Production operations:** Spring Security, Actuator, readiness probes, Micrometer, Prometheus, Docker
- **Load engineering:** bounded thread and connection pools, indexed queries, pagination, graceful shutdown, load testing

## Current project

[Spring Boot Inventory Console](https://github.com/aaron-samuvel/springboot-inventory-console) — an in-progress Java showcase using Spring MVC, JSP/JSTL, PostgreSQL, and Apache Tomcat. It includes environment-based configuration, security, migrations, health probes, metrics, bounded pools, and container deployment guidance. GitHub Actions now passes the WAR build, PostgreSQL integration tests, and container image build. A staging load test is still pending, so I am not presenting it as production-certified.

## Engineering approach

- Keep secrets and environment-specific settings outside source control.
- Make migrations, secure defaults, observability, and graceful shutdown part of the initial design.
- Tune capacity from measurements instead of assuming that default pool sizes guarantee performance.
- Document deployment and operational trade-offs clearly.

My current focus is Spring Boot, Spring MVC, XML-based servlet and Tomcat configuration, JSP, JSTL, and reliable production deployment.
