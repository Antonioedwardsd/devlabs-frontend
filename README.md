# Todo Management Application - Frontend

Este repositorio contiene el frontend de una aplicación para la gestión de tareas, construido con Next.js, TypeScript y Styled Components. La aplicación permite a los usuarios autenticados visualizar, crear, editar y eliminar tareas con una interfaz interactiva y moderna.

## Tabla de Contenidos

- [Características](#características)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Requisitos Previos](#requisitos-previos)
- [Configuración](#configuración)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Comandos Disponibles](#comandos-disponibles)
- [Testing](#testing)

---

## Características

- **Interfaz de Usuario Amigable:** Diseño intuitivo y atractivo con Styled Components.
- **CRUD de Tareas:** Crear, obtener, actualizar y eliminar tareas con sincronización al backend.
- **Autenticación:** Integración con Auth0 para gestionar usuarios.
- **Gestor de Estado Global:** Implementado con Redux Toolkit.
- **Testing:** Pruebas unitarias configuradas.

---

## Tecnologías Utilizadas

- **Next.js**
- **React**
- **TypeScript**
- **Styled Components**
- **Auth0 para autenticación**
- **Redux Toolkit para gestión del estado**

---

## Requisitos Previos

Asegúrate de tener instalados los siguientes programas:

- [Node.js](https://nodejs.org/) (versión recomendada: >= 18)
- [Yarn](https://yarnpkg.com/) o [npm](https://www.npmjs.com/)

---

## Configuración

1. Clona el repositorio:

   ```bash
   git clone https://github.com/Antonioedwardsd/devlabs-frontend
   cd proyecto-frontend
   ```

2. Instala las dependencias:

   ```bash
   npm install
   ```

3. Configura las variables de entorno. Crea un archivo `.env.local` en la raíz del proyecto basado en el siguiente ejemplo:

   ```env
   NEXT_PUBLIC_AUTH0_CLIENT_ID=tu_auth0_client_id
   NEXT_PUBLIC_AUTH0_API_AUDIENCE=tu_auth0_api_audience
   NEXT_PUBLIC_AUTH0_ISSUER=tu_auth0_issuer
   NEXT_PUBLIC_AUTH0_BASE_URL=http://localhost:3000
   NEXT_PUBLIC_AUTH0_CLIENT_SECRET=tu_auth0_client_secret
   ```

4. Inicia la aplicación en modo desarrollo:

   ```bash
   npm run dev
   ```

5. Accede a la aplicación en `http://localhost:3000`.

---

## Estructura del Proyecto

```plaintext
frontend/
├── src/
│   ├── components/          # Componentes reutilizables
│   ├── pages/               # Páginas principales de la aplicación
│   │   ├── api/             # Rutas API para la integración con el backend
│   │   ├── auth/            # Autenticación con Auth0
│   │   └── index.tsx        # Página principal
│   ├── redux/               # Configuración de Redux Toolkit
│   ├── services/            # Servicios para llamadas a la API
│   ├── styles/              # Archivos de estilos globales
│   ├── utils/               # Utilidades varias
│   └── interfaces.ts        # Tipos e interfaces
├── .env.local               # Variables de entorno
├── next.config.js           # Configuración de Next.js
├── package.json             # Dependencias y scripts
├── tsconfig.json            # Configuración de TypeScript
```

---

## Comandos Disponibles

- **Desarrollo:**
  ```bash
  npm run dev
  ```
- **Construcción para Producción:**
  ```bash
  npm run build
  ```
- **Inicio en Producción:**
  ```bash
  npm run start
  ```
- **Linter:**
  ```bash
  npm run lint
  ```

---

## Testing

Para ejecutar las pruebas unitarias:

```bash
npm test
```

---
