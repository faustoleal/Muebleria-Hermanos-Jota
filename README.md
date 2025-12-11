# Hermanos Jota V1

Proyecto final ITBA - E-commerce de muebles premium

## Descripción

Hermanos Jota es una aplicación web para la venta de muebles premium, desarrollada como proyecto para ITBA. Permite explorar productos, ver detalles, filtrar por categoría y precio, y simular compras.
Se pueden crear usuarios y dependiendo de su rol asignado tiene diferentes acciones posibles: El usuario por defecto se crea con un rol **_user_** el cual es necesario para poder acceder al carrito y realizar tus compras. Por otra lado tenemos los usuarios de rol **_admin_** el cual nos permite controlar el stock de productos(agregar, editar o eliminar un producto) y a su vez nos permite adminstrar los usuarios.

## Tecnologías

- **Frontend:** React, CSS
- **Backend:** Node.js, Express
- **Base de datos:** MongoDB
- **Otros:** Fetch API, ES Modules

## Instalación

1. Clona el repositorio:

   ```
   git clone https://github.com/faustoleal/Muebleria-Hermanos-Jota.git

   ```

2. Instala dependencias en el backend y frontend:

   ```
   cd HermanosJota/backend
   npm install

   cd client/hermanos-jota
   npm install
   ```

## Ejecución

1. Inicia el backend:

   ```
   cd backend
   npm start o npm run dev
   ```

   El backend corre en `http://localhost:3000`.

2. Inicia el frontend:
   ```
   cd client
   npm run dev
   ```
   El frontend corre en `http://localhost:5173`.

## Despliegue

- Frontend: en Vercel
- Backend: web service en Render
- Configuración de CORS incluida para comunicación entre ambos servicio

## Funcionalidades

- Listado de productos con filtros por categoría y precio
- Vista detallada de cada producto
- Contador de cantidad y simulación de compra
- Navegación entre páginas (Inicio, Productos, Contacto)
- Creación de usuarios
- Rol admin para usuarios
- Cambiar contraseña

## Estructura de carpetas

```
HermanosJota/
├── backend/
│   ├── controllers/
│   │   ├── LoginController.js
│   │   ├── ProductoController.js
│   │   └── UserController.js
│   ├── persistence/
|   |   ├── modelos/
|   |   |   ├── Producto.js
|   |   |   └── User.js
|   |   └── dbConfig.js
|   ├── routes/
|   |   ├── loginRoutes.js
|   |   ├── productRoutes.js
|   |   └── userRoutes.js
|   ├── middleware.js
|   ├── server.js
|   └── ...
├── client/hermanos-jota
|   ├── public/
|   |   └── assets
│   ├── src/
|   |   ├── api/
│   │   ├── components/
|   |   |   ├── ProtectedRoute/
|   |   |   ├── screen/
|   |   |   └── ui/
│   │   ├── context/
|   |   ├── hooks/
|   |   └── ...
│   └── ...
└── README.md
```

## Autores

- Jeronimo Cortez
- Nahuel Donatti
- Fausto Leal
- Samuel Darte
- ITBA - Proyecto Final
