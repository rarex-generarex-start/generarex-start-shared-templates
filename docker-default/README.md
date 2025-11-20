# <%= project.name %> Docker Configuration

## Usage

### Creeate .env file from .env.example

```sh
cp .env.example .env
```

Change settings according to your project

| Option               | Description                                 |
|----------------------|---------------------------------------------|
| COMPOSE_PROJECT_NAME | Docker project name, also used as subdomain |
| HOSTNAME             | First level domain                          |
| PROJECT_PATH         | Path to your project files                  |

Domains will look like `COMPOSE_PROJECT_NAME.HOSTNAME`

### Run docker-compose

```sh
docker-compose up --build -d
```
