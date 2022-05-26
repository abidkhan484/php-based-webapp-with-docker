# Containerization MySQL for local development

## Prerequisites
- Virtual Machine
- Docker
- Docker Compose

## Project Tree
```sh
.
├── README.md
├── .env.example
├── docker-compose.yml
├── mysql_custom.cnf
├── mysql_datadir/
```
## Procedures
1. After cloning the Git repository and changing to the directory
```sh
git clone https://github.com/abidkhan484/php-webapp-with-docker.git
cd php-webapp-with-docker/mysql
```
1. Copy the environment file.
```sh
cp .env.example .env
```
2. Start the servers with the below command.
```sh
docker-compose up -d
```
3. Open your favorite browser and access Phpmyadmin:
```sh
http://localhost:8080
```
4. Stop and clear services
```sh
docker-compose down -v
```
## Useful Commands
1. Access from the host machine using port/ credentials specified in the env file
```sh
mysql -h 127.0.0.1 -P 33006 -u root -p
```

## Conclusion
Change the `mysql_custom.cnf` or the `.env` file according to your need.
