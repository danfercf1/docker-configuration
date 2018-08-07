DOCKER configuration to some habitual services

# Check the configuration

`docker-compose config`

or

`docker-compose -f docker-compose-file config`

# Wordpress
## Services:
* MariaDb: Data base
* Adminer: Data base web based administrator
* Wordpress: Blog content manager
## Systemd Service
    1. Copy the service wordpress.service to /lib/systemd/system/
    2. Copy docker-compose.yml and .env files to /etc/docker-compose/services/service-name/
    3. Enable the service: sudo systemctl enable service_name.service
    4. Run the service: sudo service service_name start
