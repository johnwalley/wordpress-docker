A docker compose file for setting up Wordpress.

Example environment variables:

db.env

    MYSQL_ROOT_PASSWORD=example
    MYSQL_DATABASE=wordpress
    MYSQL_USER=wordpress
    MYSQL_PASSWORD=example

wordpress.env

    WORDPRESS_DB_HOST=db:3306
    WORDPRESS_DB_NAME=wordpress
    WORDPRESS_DB_USER=wordpress
    WORDPRESS_DB_PASSWORD=example

backup.env

    MYSQL_ENV_MYSQL_USER=wordpress
    MYSQL_ENV_MYSQL_DATABASE=wordpress
    MYSQL_ENV_MYSQL_PASSWORD=example
    MYSQL_PORT_3306_TCP_PORT=3306