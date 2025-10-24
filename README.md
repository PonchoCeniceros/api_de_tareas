# API de Tareas

El siguiente proyecto es una API para gestionar una lista de tareas. Esta desarrollado en el stck MERN con Typescript y sigue de forma general los preceptos de la arquitectura limpia. La estructura del directorio `src` en el backend refleja las capas de `Infraestructura -> Aplicación -> Dominio`:

```
/src
│
├───auth/                # Módulo de autenticación (infraestructura)
│   ├───controllers.ts   # Aquí también se embebe la capa de aplicación
│   ├───middlewares.ts
│   └───routes.ts
│
├───tasks/               # Módulo de las tareas (infraestructura)
│   ├───controllers.ts   # Aquí también se embebe la capa de aplicación
│   └───routes.ts
│
├───domain/              # Entidades y reglas de negocio (dominio)
│   ├───apiResponse.ts
│   ├───jwtPayload.ts
│   ├───role.ts
│   ├───session.ts
│   └───user.ts
│
├───models/              # Esquemas y modelos de la base de datos (infraestructura)
│   └───user.model.ts
│
├───services/            # Conectores a servicios externos (infraestructura)
│   └───mongo.connector.ts
├───api.ts               # Punto de entrada y configuración de Express
└───index.ts             # Script de inicio del servidor
```


## Iniciar con NPM

1.  Instalar dependencias:
    ```bash
    npm install
    ```
2.  Construir el proyecto:
    ```bash
    npm run build
    ```
3.  Iniciar el servidor:
    ```bash
    npm start
    ```
4.  Para desarrollo, puedes usar:
    ```bash
    npm run dev
    ```
