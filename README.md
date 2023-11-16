# skeleton-srp
### Desarrollo con Docker, Java, React, Zsh, Pnpm, PostgreSQL y PgAdmin

Este repositorio proporciona una estructura lista para el desarrollo de una aplicación que utiliza Java para el backend, React para el frontend, PostgreSQL como base de datos y PgAdmin como cliente de base de datos. Además, se incluyen configuraciones para el uso de Docker, Zsh con plugins útiles, y Pnpm como gestor de paquetes.

## Estructura del Proyecto

### Backend (Java)

El backend se encuentra en la carpeta `backend`. Se utiliza un contenedor Docker para gestionar las dependencias y ejecutar la aplicación Java. El archivo `Dockerfile.dev` contiene las instrucciones para construir el contenedor.

- **Puerto:** 8080
- **Rutas:** Los archivos y código fuente del backend están en la carpeta `/app/backend`.

### Frontend (React)

El frontend está ubicado en la carpeta `frontend`. Al igual que el backend, se utiliza un contenedor Docker con el archivo `Dockerfile.dev` para gestionar las dependencias y ejecutar la aplicación React.

- **Puerto:** 5173
- **Rutas:** Los archivos y código fuente del frontend están en la carpeta `/app/frontend`.

### Base de Datos (PostgreSQL)

La base de datos PostgreSQL está configurada en el contenedor `database`. Se inicializa con un usuario y contraseña específicos definidos en las variables de entorno.

- **Puerto:** 5432
- **Usuario:** postgres
- **Contraseña:** postgres
- **Base de Datos:** exampledb

### Cliente de Base de Datos (PgAdmin)

El cliente de PostgreSQL, PgAdmin, se encuentra en el contenedor `dbclient`. Proporciona una interfaz web para gestionar la base de datos PostgreSQL.

- **Puerto:** 5050
- **Usuario:** pgadmin4@pgadmin.org
- **Contraseña:** admin

### Configuraciones Adicionales

- **Zsh:** La estructura incluye configuraciones para Zsh, un shell de Unix, que mejora la productividad con sus características y plugins.

- **Pnpm:** Pnpm se utiliza como gestor de paquetes para el frontend React, asegurando una gestión eficiente de las dependencias.

## Instrucciones de Uso

1. Clona este repositorio.

```bash
git clone <URL_DEL_REPOSITORIO>
cd <NOMBRE_DEL_REPOSITORIO>
