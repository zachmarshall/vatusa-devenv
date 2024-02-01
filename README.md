# vatusa-devenv

Creates a simple docker-compose based development environment for running integrated VATUSA backend stack.

## Requirements

This environment currently requires the following Docker images:

* `rabbitmq:3-management`. This is pulled from Docker hub automatically.
* `taskrunner:latest`. For now, it's expected that this is built locally. See [VATUSA/TaskRunner](https://github.com/VATUSA/TaskRunner) to build.

## Running

To run: `docker compose -f compose.yaml up -d --build`

## Debugging

This environment currently exposes the RabbitMQ management UI on host port `:8080`.