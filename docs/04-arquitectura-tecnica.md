# 🌸 Flor Studio - Arquitectura Técnica

## Introducción

Este documento define la arquitectura tecnológica que utilizará Flor Studio.

La aplicación será desarrollada como una Aplicación Web Progresiva (PWA), permitiendo instalarse en dispositivos móviles como una aplicación nativa.

---

# Arquitectura general

La aplicación estará dividida en tres capas:

## Frontend

Responsable de la interfaz visual y experiencia del usuario.

Tecnologías:

- Next.js
- React
- TypeScript
- Tailwind CSS

Funciones:

- Pantallas.
- Formularios.
- Dashboard.
- Visualización de datos.
- Interacción del usuario.

---

## Backend

Responsable de la lógica del sistema y comunicación con la base de datos.

Tecnología:

- Supabase

Funciones:

- Autenticación.
- Gestión de usuarios.
- Consultas.
- Seguridad.
- APIs.

---

## Base de datos

Motor:

PostgreSQL mediante Supabase.

Responsable de almacenar:

- Usuarios.
- Materiales.
- Productos.
- Recetas.
- Pedidos.
- Clientes.
- Ventas.

---

Estructura del proyecto

La aplicación tendrá la siguiente organización:

flor-studio-app

frontend/

backend/

database/

docs/

assets/
---

# Frontend

Framework:

Next.js

Lenguaje:

TypeScript

Estilos:

Tailwind CSS


Componentes principales:

- Navbar.
- Sidebar.
- Dashboard.
- Formularios.
- Tablas.
- Tarjetas estadísticas.

---

# Backend

Supabase proporcionará:

## Authentication

Sistema de inicio de sesión.

## Database

Base PostgreSQL.

## Storage

Almacenamiento de imágenes:

- Productos.
- Materiales.
- Clientes.

## API

Comunicación entre frontend y datos.

---

# Aplicación PWA

Flor Studio podrá instalarse en Android.

Características:

- Icono en pantalla principal.
- Funcionamiento similar a una app.
- Diseño adaptable.
- Posibilidad futura de modo offline.

---

# Seguridad

Se implementará:

- Autenticación de usuarios.
- Control de permisos.
- Protección de datos.
- Variables de entorno.

---

# Herramientas de desarrollo

Control de versiones:

GitHub

Editor recomendado:

Visual Studio Code

Gestión del proyecto:

Git

---

# Futuras integraciones

La arquitectura permitirá agregar:

- WhatsApp Business.
- Notificaciones.
- Pagos online.
- Catálogo público.
- Inteligencia artificial Flora.
