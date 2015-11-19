# Deployment

### Environment Variables

```sh
$ export SECRET_KEY_BASE="LONG_HASH"
$ export NEW_RELIC_LICENSE_KEY="KEY"
```

### Start

```sh
# Start containers
$ docker-compose up -d

# Database initial setup
$ docker-compose run web rake db:setup

# Just migrate
$ docker-compose run web rake db:migrate

# See logs
$ docker-compose logs

# Stop
$ docker-compose stop
```
