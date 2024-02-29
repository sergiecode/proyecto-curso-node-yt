# NODE JS: API REST (CRUD) con PostgreSQL y JWT

Este repositorio tiene una API-REST realizada con Node.js y PostgreSQL la cual nos sirve para hacer un CRUD (alta, baja, modificación y lectura) sobre usuarios utilizando autenticación vía token con JWT (Json Web Token). Este repositorio pertenece al curso de NODE.JS desde Cero que puedes ver aquí:  [https://youtu.be/I17ln313Pjk](https://youtu.be/I17ln313Pjk)

## Uso

1.  Cloná el repositorio haciendo `git clone https://github.com/sergiecode/proyecto-curso-node-yt`
2.  Abrí el proyecto en su editor de código
3.  Instalá de los paquetes y módulos requeridos: `npm install`
4.  Agrega las variables de entorno que correspondan usando como plantilla `.env.template`
5.  Teniendo abierto Docker Desktop ejecuta `docker compose up -d`
6. Levantá el servidor haciendo `npm run dev`

## Requiere:

-   **NODE**: Se debe instalar NODE en el sistema operativo
-   **DOCKER**: Para poder levantar la imágen de Mongo en el contenedor
-   **GIT**: Debe tener Instalado GIT

## Pasos para  configurar un proyecto como este:
1. `npm init -y`
2. `npm install express jsonwebtoken bcrypt @prisma/client dotenv typescript`
3. `npm install --save-dev ts-node-dev @types/express @types/jsonwebtoken @types/bcrypt @types/node rimraf prisma`
4. `npx tsc --init --outDir dist/ --rootDir src`
5. Agregar carpetas excluídas e incluídas al archivo de configuración de TypeScript `"exclude": ["node_modules","dist" ],
"include": ["src"] `
6. `npx prisma init`
7. `npx prisma generate`
8. Agregar los modelos en `schema.prisma`
9. `npmx prisma migrate dev`
10. `docker-compose up -d` 
11. Agregar los siguientes scripts: `"dev": "tsnd --respawn --clear src/app.ts",
  "build": "rimraf ./dist && tsc",
  "start": "npm run build && node dist/app.js"`

## METHODS
### POST:
http://localhost:3000/auth/register
http://localhost:3000/users
http://localhost:3000/auth/login
### GET ALL
http://localhost:3000/users
### GET PUT DELETE BY ID
http://localhost:3000/users/:id

## Acerca del curso de  [NODE.JS desde Cero en YouTube](https://youtu.be/I17ln313Pjk)
¡Primer curso del 2024, primer curso de Backend del canal! 

Tal cual les prometí, después de un increíble 2023 a full Frontend, este año me voy a centrar en el backend y bases de datos. Este curso no solo te enseñará Node.js sino que también abarca Express, MongoDB, PostgreSQL, Docker, Mongoose, Prisma, Railway, Github, entre otros.

¡Los cursos de JavaScript y React superaron ampliamente los 100k y muchísima gente me estaba pidiendo el de NodeJS para completar su stack y por fin ha llegado!

## Me pueden encontrar en: 

[Canal de Youtube | Sergie Code](https://www.youtube.com/@SergieCode)

[Github | Sergie Code](https://github.com/sergiecode)

[LinkedIn | Sergie Code](https://www.linkedin.com/in/sergiecode/)

[Instagram | Sergie Code](https://www.instagram.com/sergiecode)
