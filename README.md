# eea.docker.postgres_data

usage: 

create the volume (/var/lib//pgsql/data and /var/lib/postgresql/data): 

    docker run -d --name <app>_postgres_data eeacms/postgres-data

usage it with postgres example:

    docker run --restart=always --name <app>_postgres --volumes-from=<app>_postgres_data -e POSTGRES_ROOT_PASSWORD=<mypassword> -d postgresql
