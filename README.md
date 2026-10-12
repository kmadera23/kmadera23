Estudiante de Ingeniería de Sistemas y desarrollador full stack. Construyo software de principio a fin: API, base de datos, interfaz y despliegue.

## Stack

**Backend**
![Java](https://img.shields.io/badge/Java_17-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat&logo=springsecurity&logoColor=white)

**Frontend**
![React](https://img.shields.io/badge/React_18-20232A?style=flat&logo=react&logoColor=61DAFB)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white)

**Datos e infraestructura**
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)

## Proyectos destacados: 

**SoftVia POS:**
Sistema de punto de venta para comercios: ventas, inventario, caja, roles y reportes.

- **API REST** con Spring Boot 3.4, JPA/Hibernate y documentación OpenAPI.
- **Seguridad:** autenticación con JWT, roles y permisos, y límite de peticiones con Bucket4j.
- **Base de datos** versionada con Flyway (más de 80 migraciones), compatible con MySQL y PostgreSQL.
- **Tiempo real** con WebSocket y caché con Redis.
- **Frontend en React** con TanStack Query, gráficos con Recharts y soporte offline como PWA (Workbox + IndexedDB).
- **Calidad:** más de 90 clases de prueba con JUnit y JaCoCo, pruebas E2E con Playwright y CI en GitHub Actions.
- **Observabilidad:** métricas con Micrometer, Prometheus y OpenTelemetry.
- **Exportación** de reportes a Excel, CSV y PDF.

**DGII RNC API:**
API REST para consultar contribuyentes de la DGII (República Dominicana) por RNC o cédula, y buscarlos por nombre.

Sincronización diaria del archivo oficial de la DGII a PostgreSQL (cerca de 791 mil contribuyentes).
Consulta en vivo opcional contra el portal, con caché y circuit breaker.
Autenticación por API key con límite de peticiones por clave.
Flask con documentación Swagger, migraciones con Alembic y scheduler para la sincronización.
Empaquetado con Docker (build multietapa) y gestión de dependencias con uv.
Pruebas con pytest, tipado estricto con mypy y linting con Ruff.
Servicio no oficial: los datos provienen de publicaciones de la DGII.

**ArqVia CRM:**
CRM SaaS pensado para firmas de arquitectos que hoy trabajan con Excel, con un núcleo reutilizable para otras industrias. Actualmente en fase de desarrollo.

Backend en Spring Boot 3.5 y Java 21, con Spring Security y validación.
Migraciones con Flyway sobre PostgreSQL y pruebas de integración con Testcontainers.
Frontend en React 19 con TypeScript y Vite, probado con Vitest y Testing Library.
Entorno local reproducible con Docker Compose.


## Cómo trabajo

- **APIs documentadas desde el inicio:** contratos claros con OpenAPI/Swagger, validación de entrada y autenticación por JWT o API key.
- **Base de datos con historial:** cada cambio de esquema es una migración versionada (Flyway, Alembic), nunca un ajuste manual.
- **Pruebas antes de confiar:** unitarias, de integración con bases de datos reales (Testcontainers) y E2E, con CI que las corre en cada cambio.
- **Entornos reproducibles:** todo levanta con Docker Compose, con healthchecks y métricas para saber qué pasa en producción.
- **Seguridad en el día a día:** límite de peticiones, roles y permisos, y escaneo de secretos con gitleaks para que una clave no llegue al repositorio.
- **Respaldos y recuperación:** copias automáticas programadas y scripts de verificación de restauración, porque un respaldo que no se prueba no cuenta.
- **Runbooks:** guía de operación para despliegue, incidentes y mantenimiento, escrita para que otra persona pueda seguirla.
