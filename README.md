# FutStars ⚽

Aplicación web de fútbol desarrollada como proyecto académico DAM.

## 🛠️ Stack Tecnológico

### Frontend
- **Framework**: Astro + React 18
- **Lenguaje**: TypeScript
- **Estilos**: Tailwind CSS
- **HTTP Client**: Axios
- **Despliegue**: Vercel

### Backend
- **Framework**: Spring Boot 3.2
- **Lenguaje**: Java 21
- **Seguridad**: Spring Security + JWT
- **ORM**: Hibernate/JPA
- **API Docs**: Swagger/OpenAPI
- **Despliegue**: Render

### Base de Datos
- **Motor**: PostgreSQL 15
- **Proveedor**: Supabase

### API Externa
- **Proveedor**: API-Football (v3)

## 📦 Estructura del Proyecto

\`\`\`
futstars/
├── frontend/          # Aplicación Astro + React
├── backend/           # API REST Spring Boot
├── docs/             # Documentación técnica
│   └── decisiones-arquitectura.md
└── README.md
\`\`\`

## 🚀 Inicio Rápido

### Requisitos Previos
- Node.js 18+
- Java 21 (JDK)
- Maven 3.9+
- PostgreSQL 15 (o cuenta Supabase)
- Git

### Instalación

#### Backend
\`\`\`bash
cd backend
./mvnw spring-boot:run
\`\`\`

#### Frontend
\`\`\`bash
cd frontend
npm install
npm run dev
\`\`\`

### Variables de Entorno
Copiar `.env.example` a `.env` y configurar:
- `API_FOOTBALL_KEY`: Tu API key de API-Football
- `DATABASE_URL`: URL de conexión a PostgreSQL
- `JWT_SECRET`: Secreto para firmar tokens JWT

## 🔐 Acceso a la API

### Endpoints Públicos
- `POST /api/auth/register` - Registro de usuario
- `POST /api/auth/login` - Inicio de sesión
- `GET /api/leagues` - Listar ligas
- `GET /api/teams` - Listar equipos

### Endpoints Protegidos
- `GET /api/users/me` - Perfil del usuario
- `GET /api/favorites` - Listar favoritos
- `POST /api/favorites` - Añadir favorito
- `DELETE /api/favorites/{id}` - Eliminar favorito

## 📊 Estado del Proyecto

- [x] Arquitectura definida
- [x] Estructura del monorepo
- [ ] Configuración inicial del backend
- [ ] Configuración inicial del frontend
- [ ] Autenticación JWT
- [ ] Integración con API-Football
- [ ] CRUD de favoritos
- [ ] Despliegue

## 👥 Equipo

Tres desarrolladores - Proyecto académico DAM

## 📄 Licencia

Este proyecto es para fines educativos.