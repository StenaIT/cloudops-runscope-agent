# cloudops-runscope-agent

A docker image for running the [runscope agent](https://www.runscope.com/docs/radar/agent).

[![Docker Automated build](https://img.shields.io/docker/automated/stena/cloudops-runscope-agent.svg?style=for-the-badge)](https://hub.docker.com/r/stena/cloudops-runscope-agent/)
[![Docker Build Status](https://img.shields.io/docker/build/stena/cloudops-runscope-agent.svg?style=for-the-badge)](https://hub.docker.com/r/stena/cloudops-runscope-agent/)
[![MicroBadger Size](https://img.shields.io/microbadger/image-size/stena/cloudops-runscope-agent.svg?style=for-the-badge)](https://hub.docker.com/r/stena/cloudops-runscope-agent/)
[![Docker Pulls](https://img.shields.io/docker/pulls/stena/cloudops-runscope-agent.svg?style=for-the-badge)](https://hub.docker.com/r/stena/cloudops-runscope-agent/)

## Configuration

See the documentation for runscope agent for information on how to get the required configuration values.

Environment Variable | Description                    | Default                 | Required
---------------------|--------------------------------|-------------------------|---------
TOKEN                | The runscope agent token       | -                       | true
AGENT_ID             | The runscope agent id          | -                       | true
TEAM_ID              | The runscope team id           | -                       | true
NAME                 | The name of the runscope agent | cloudops-runscope-agent | false
TIMEOUT              | Connection idle timeout        | 20                      | false
DISCONNECT_TIMEOUT   | Disconnect timeout             | 5                       | false
THREADS              | Number of worker threads       | 3                       | false
CA_FILE              | CA certificate file            | -                       | false

## Using the docker image

```bash
docker run --rm \
  -e NAME=name \
  -e TOKEN=token \
  -e AGENT_ID=agent_id \
  -e TEAM_ID=team_id \
  stena/cloudops-runscope-agent
```
