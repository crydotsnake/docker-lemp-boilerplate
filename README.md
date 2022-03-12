# Docker-Lemp Boilerplate

Run Nginx, php-fpm, PHPMyAdmin, and MariaDB using [Docker]

## Requirements

Install [Docker]

## Usage

```bash
docker compose up -d
docker compose logs
docker compose stop
docker compose rm
```

Since Compose V2 compose is now integrated directly in Docker. Read more [here](https://docs.docker.com/compose/cli-command/)

### URLs

- http://localhost:8081/ (Project URL)
- http://localhost:8080/ (PHPMyAdmin)

---

[Docker]: https://www.docker.com/

Credits:
- Based on [docker-lemp](https://github.com/stucki/docker-lemp) by [Michael Stucki](https://github.com/stucki)