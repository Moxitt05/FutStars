# FutStars ⚽

Aplicación web full stack de fútbol desarrollada como proyecto académico de DAM y orientada también como proyecto de portfolio profesional.

El objetivo de FutStars es consultar información futbolística mediante API-Football y ofrecer funcionalidades propias para usuarios registrados.

---

## 🏗️ Arquitectura

```
Frontend (Astro + React)
          |
          | HTTP REST
          ↓
Backend (Spring Boot)
          |
          ├── PostgreSQL (Supabase)
          |
          └── API-Football
```

La API externa nunca será consumida directamente desde el frontend.  
Todas las peticiones a API-Football pasan por el backend.

---

## 🛠️ Stack Tecnológico

## Frontend

- **Framework**: Astro + React
- **Lenguaje**: TypeScript
- **Estilos**: Tailwind CSS
- **HTTP Client**: Axios
- **Despliegue**: Vercel

## Backend

- **Framework**: Spring Boot 3
- **Lenguaje**: Java 21
- **Seguridad**: Spring Security + JWT
- **ORM**: Hibernate / Spring Data JPA
- **Cliente HTTP**: WebClient
- **API Docs**: Swagger / OpenAPI
- **Gestor de dependencias**: Maven
- **Despliegue**: Render

## Base de Datos

- **Motor**: PostgreSQL
- **Proveedor**: Supabase

## API Externa

- **Proveedor**: API-Football (v3)

---

## 📦 Estructura del Proyecto

```
futstars/
├── frontend/              # Aplicación Astro + React
├── backend/               # API REST Spring Boot
├── docs/                  # Documentación técnica
│   └── decisiones-arquitectura.md
└── README.md
```

---

## 🚀 Inicio Rápido

## Requisitos Previos

- Node.js 18+
- Java 21 (JDK)
- Maven 3.9+
- PostgreSQL / Cuenta Supabase
- Git

---

## Instalación

### Backend

```
cd backend

./mvnw spring-boot:run
```

En Windows:

```
.\mvnw.cmd spring-boot:run
```

Backend disponible en:

```
http://localhost:8080
```

---

### Frontend

```
cd frontend

npm install

npm run dev
```

Frontend disponible en:

```
http://localhost:4321
```

---

## 🔐 Variables de Entorno

Crear un archivo `.env` a partir de `.env.example`.

Variables previstas:

### Backend

```
DATABASE_URL=
DATABASE_USERNAME=
DATABASE_PASSWORD=
API_FOOTBALL_KEY=
JWT_SECRET=
```

### Frontend

```
PUBLIC_API_URL=
```

---

## 🔌 API REST

### Endpoints públicos previstos

```
POST /api/auth/register
POST /api/auth/login

GET /api/leagues
GET /api/teams
GET /api/players
GET /api/matches
```

---

### Endpoints protegidos previstos

```
GET /api/users/me

GET /api/favorites

POST /api/favorites

DELETE /api/favorites/{id}
```

---

## 📊 Estado del Proyecto

- [x] Arquitectura definida
- [x] Monorepo configurado
- [x] Backend Spring Boot creado
- [x] Frontend Astro creado
- [x] API REST inicial funcionando
- [ ] Configuración PostgreSQL / Supabase
- [ ] Modelo de datos JPA
- [ ] Autenticación JWT
- [ ] Integración con API-Football
- [ ] Sistema de favoritos
- [ ] Gráficas y estadísticas
- [ ] Despliegue

---

## 👥 Equipo

Proyecto desarrollado por tres estudiantes del ciclo DAM.

El desarrollo se realiza de forma colaborativa, trabajando sobre frontend, backend, base de datos, autenticación e integración con APIs.

---

## 📄 Licencia

Proyecto desarrollado con fines educativos como parte del ciclo de Desarrollo de Aplicaciones Multiplataforma (DAM).