### Steps

```
npm install -g @nestjs/cli

nest new nest-crud-app

cd nest-crud-app

npm i pg typeorm @nestjs/typeorm @nestjs/config

code .

npm start

# Create the NestJS application
nest g module users
nest g controller users
nest g service users
touch src/users/user.entity.ts

# User Entity
src/users/user.entity.ts

# User Service
src/users/users.service.ts

# User Controller
src/users/users.controller.ts

# User Module
src/users/users.module.ts

# Update the Main Module
src/app.module.ts

# Dockerize the application
touch Dockerfile .dockerignore docker-compose.yml

.dockerignore
Dockerfile
docker-compose.yml

# Run the Postgres service
docker compose up -d db
docker ps -a

# Build the Nest app image
docker compose build

# Run the Nest app
docker compose up

# Test the application
GET request to localhost:3000/users

POST request to localhost:3000/users
{
    "name": "aaa",
    "email": "aaa@mail"
}

GET request to localhost:3000/users

GET request to localhost:3000/users/2

PUT request to localhost:3000/users/2
{
  "name":"me",
  "email":"me@mail"
}

DELETE request to localhost:3000/users/3

```

### References

- https://medium.com/@akashjha9041/typescript-crud-rest-api-using-nest-js-typeorm-postgres-docker-and-docker-compose-c10ab00ebe48
