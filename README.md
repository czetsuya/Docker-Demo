# Docker

This project deploys a JavaEE war project into Wildfly running on docker with database, logging tools, db tools and Keycloak.

Note that Keycloak is not connected to Wildfly. If needed Keycloak adapter must be installed on Wildfly with the correct client configuration.

This project installs:

 * Postgresql
 * Adminer
 * Tailon
 * Wildfly
 * Keycloak

It deploys a JavaEE war from Github which access the Postgresql database.

## Windows

Update the PWD variable value in .env.

## Ubuntu

Remove the PWD variable, Ubuntu/Linux already provide this variable.

To run: 
>docker-compose up --build

In your browser you may open the following url:

 * http://localhost:8080/javaee6-webapp
 * http://localhost:8081 - Adminer
 * http://localhost:8082 - Tailon
 * http://localhost:8083 - Keycloak
