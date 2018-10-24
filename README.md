# cloudops-runscope-agent

A docker image for running the [runscope agent](https://www.runscope.com/docs/radar/agent).

## Configuration

See the documentation for runscope agent for information on how to get the required configuration values.

Environment Variable | Description                    | Default
---------------------|--------------------------------|------------------------
NAME                 | The name of the runscope agent | cloudops-runscope-agent
TOKEN                | The runscope agent token       | -
AGENT_ID             | The runscope agent id          | -
TEAM_ID              | The runscope team id           | -

## Using the docker image

```bash
docker run --rm \
  -e NAME=name \
  -e TOKEN=token \
  -e AGENT_ID=agent_id \
  -e TEAM_ID=team_id \
  stena/cloudops-runscope-agent
```
