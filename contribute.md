## Docker installation
- Install docker
- create a network - docker network create user_project
- start postgres
  - docker run --network user_project --name postgres -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres
- Build the image - `docker build --network=host  -t user-project .`
- start the image - `docker run -e DATABASE_URL=postgresql://postgres:mysecretpassword@postgres:5432/postgres --network user_project -p 3000:3000 user-project`

## Docker compose
- Install docker
- run `docker-compose up` 