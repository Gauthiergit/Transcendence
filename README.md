# Transcendence

The last project of 42cursus

## Execution

1. You need to create the directory for the database
````sh
mkdir database
````
2. You need to change the path of each volume in the file `docker-compose.yml` in volume section & device for each one: PostgreSQL to the directory you want to create and Django to the directory `transcendence_srcs`

3. This version use auto-signed certificat

4. You need to fill variables in .env. Concerning the 2FA, we use gmail account so you must put an existing gmail in EMAIL_HOST_USER. Next you need to generate a secret key from this mail and put it in EMAIL_HOST_PASSWORD.

5. You can execute the docker
````sh
make
````

## Access
The website is accesible from : `https://localhost/`

The administration interface from : `https://localhost/admin`

The monitoring dashboard with grafana from : `localhost:3000` 
