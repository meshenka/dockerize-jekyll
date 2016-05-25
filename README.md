# Dockerize Jekyll

This is a very simple container to host jekyll based website

Dump your jekyll source in .
Add
```yaml
exclude: [docker-compose.yml]
```

to your `_config.yml` file to avoid exposing docker config in the website

Build your project

```bash
jekyll build
```

Build the container

```bash
docker-compose up
```

And see the result at [http://localhost:8080](http://localhost:8080 "Local docker container")
