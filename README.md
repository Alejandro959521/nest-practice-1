<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

# Ejecutar en desarrollo
1. clonar el repo 
2. Ejecutar el siguiente comando... 
````
yarn install
````
3. tener Nest CLI instalado... 
````
npm install i -g @nestjs/cli
````
4. levantar la base de datos... 
````
docker-compose up -d
````
5. clonar el archivo .env.template y renombrar la copia .env

6. llenar las variables de entorno definidas en el .env

7. Ejecutar la aplición en dev:

````
yar start:dev
````

8. Reconstruir la base de datos con la semilla 
````
http://localhost:3000/api/v2/seed
````

## Stack usado
* MongoDB
* Nest

# production Build 
1. Crear el archivo  ```.env.prod```
2. Llenar las variables de entorno de prod
3. Crear la nueva imagen

````
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
````
