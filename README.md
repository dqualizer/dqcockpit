# dqcockpit

A more detailed description of this component's architecture is provided in the [arc42 document](https://dqualizer.github.io/dqualizer).

## Usage
* This package is published via a GitHub Workflow to [ghcr.io](https://github.com/dqualizer/dqcockpit/pkgs/container/dqcockpit)
### Docker Compose
* `docker pull ghcr.io/dqualizer/dqcockpit`
* `docker compose up -d`

### Docker
* `docker run --env DOCKER_INFLUXDB_INIT_BUCKET=my-bucket ghcr.io/dqualizer/dqcockpit:latest`

## How to build
### Docker
* `docker buildx build -f grafana/Dockerfile --tag ghcr.io/dqualizer/dqcockpit:latest .`

### Deploy to Packages
* There is a GitHub action set up, that automatically pushes the dqCockpit image to [Github Container Registry](https://github.com/dqualizer/dqcockpit/pkgs/container/dqcockpit)

## Passwords
| Service   | Username | Password |
| --------- | -------- | -------- |
| dqcockpit | admin    | demo     |
