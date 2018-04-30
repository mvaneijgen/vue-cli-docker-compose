# vue-cli-docker-compose

A simple docker compose file to create a new vue-cli project and run in in the same container after it is created.

## Simple

Using [ebiven/docker-vue-cli](https://github.com/ebiven/docker-vue-cli) this is a simple docker-compose file that mounts the PWD as the location where the new
vue-cli generated project will be located. It is intended to be run with `docker-compose run ...`.

### Usage

**Step one**

```commandline
docker-compose run web vue init webpack app
```

Creating network `vueclidockercompose_default` with the default driver. This will install Vue 2.x version of the template.

**Step two**

```
docker-compose up
```

Runs the current generated Vue.js app on localhost `http://localhost:8080` and regenerates each time you edit something in the `/app` folder on your local machine.
