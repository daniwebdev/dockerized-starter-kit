# DOCKERIZED STARTERKIT

## Setup

- Clone this repo with `--recursive-submodules`
  
  ```bash
  git clone --recurse-submodules https://github.com/daniwebdev/dockerized-starter-kit.git
  ```

- Copy `./.env.example` to `./.env`
- Copy `backend/.env.example` to `backend/.env`
- run docker compose

  ```bash
  docker compose up -d
  ```

- make sure node dependencies are installed properly with checking log for `backend` and `frontend` containers.
- and run backend migration

  ```bash
  docker compose exec backend yarn migration:run
  ```
