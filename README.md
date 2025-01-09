<h2 align="center">
  Desafio Docker: Curso Devops Pro
</h2>
<br>

---

<p align="left">
  <img src="https://img.shields.io/static/v1?label=Tipo&message=Desafio&color=8257E5&labelColor=000000" alt="Desafio" />
</p>

#### Desafio 1 - Banco de Dados PostgreSQL:

**comando:**

```
docker run -d \
--name postgres_curso_docker \
-e POSTGRES_DB=curso_docker \
-e POSTGRES_USER=docker_usr \
-e POSTGRES_PASSWORD=docker_pwd \
-p 5437:5432 \
postgres:latest
```
**Acessar, DBeaver ou outro:**

- Host: localhost
- Port: 5437
- Database: curso_docker
- username: docker_usr
- password: docker_pwd


---

#### Desafio 2 - Banco de Dados MySQL:

**comando:**

```
docker run -d \
--name mysql_curso_docker \
-e MYSQL_DATABASE=docker_db \
-e MYSQL_USER=docker_usr \
-e MYSQL_PASSWORD=docker_pwd \
-e MYSQL_ROOT_PASSWORD=docker_pwd \
-p 3307:3306 \
mysql:latest
```
**Acessar, DBeaver ou outro:**

- Host: localhost
- Port: 3307
- Database: docker_db
- username: docker_usr
- password: docker_pwd

---

#### Desafio 3 - Banco de Dados MongoDB:

**comando:**

```
docker run -d \
--name mongodb_curso_docker \
-e MONGO_INITDB_ROOT_USERNAME=mongo_usr \
-e MONGO_INITDB_ROOT_PASSWORD=mongo_pwd \
-p 27019:27017 \
mongo:latest
```
**Acessar, MongoDB Compass:**

- mongodb://mongo_usr:mongo_pwd@localhost:27019/


