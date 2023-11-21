# docker-gemstash

A RubyGems.org cache and private gem server.

## Usage

### Basic

```
$ docker run \
  --publish=9292:9292 \
  zappi/gemstash:<VERSION>
```

### Advanced

#### SQLite

See `docker-compose.sqlite.yml` for an example of how to use SQLite. To run:

```console
$ export COMPOSE_FILE="docker-compose.sqlite.yml"
$ docker-compose up -d
$ docker-compose ps
           Name                         Command               State           Ports
--------------------------------------------------------------------------------------------
docker-gemstash_gemstash_1   /entrypoint.sh bundle exec ...   Up      0.0.0.0:9292->9292/tcp
```

#### PostgreSQL

See `docker-compose.postgres.yml` for an example of how to use PostgreSQL. To run:

```console
$ export COMPOSE_FILE="docker-compose.postgres.yml"
$ docker-compose up -d
$ docker-compose ps
           Name                         Command               State           Ports
--------------------------------------------------------------------------------------------
docker-gemstash_gemstash_1   /entrypoint.sh bundle exec ...   Up      0.0.0.0:9292->9292/tcp
docker-gemstash_postgres_1   docker-entrypoint.sh postgres    Up      5432/tcp
```
