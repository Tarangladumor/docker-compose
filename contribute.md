## Docker installation
- Install docker
- start postgres
  - docker run -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres
- Build the image - `docker build -t user-project.`
- start the image - `docker run -p 3000:3000 user-project`

## Docker compose
- Install docker
- run `docker-compose up` 