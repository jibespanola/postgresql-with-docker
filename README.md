# postgresql-with-docker
Configure `docker-compose.yml` environment variables to fit your needs
#### Run this command to set up both Postgresql and PGadmin:
`docker-compose up`
#### stop all containers, volumes, and images from up:
`docker-compose down`

## PGAdmin server configuration:
1. Login to localhost (based on the ports assigned in `docker-compose.yml`)
   * Enter username and password defined in `dpage/pgadmin4` service in `docker-compose.yml`
2. Create server
   * Connection: Enter variables defined in `db` service in `docker-compose.yml`
      * Host name/address: db
      * username: postgres

## To persist data, uncomment volumes lines 
Pick between **volume mount** or **bind mount**.
[When to use volume mount or bind mount?](https://docs.docker.com/storage/)
