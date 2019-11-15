## laravel-docker

This will helps you to run your laravel application.

### Instruction:

- Copy all the files into your laravel root directory.

##### If you want to customize the docker image please do the following changes:
- Modify the `docker-compose.yml` file with your required information. *UPDATE DATABASE CREDENTIAL*
- Modify `Dockerfile` for installing any additional packages.
- Modify `.docker/nginx/conf.d/app.conf` for webserver.
- Modify `.docker/php/local.ini` for necessary php related changes.
- Modify `.docker/mssql/my.cnf` for mysql changes.

Finally, *RUN* the following command to build the docker image:
```bash
docker-compose up -d
```

##### To rebuild the image please use the following command:
```bash
docker-compose up -d --build
```
