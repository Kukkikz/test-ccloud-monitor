# test-ccloud-monitor
Use `export` command to set parameter in docker-compose file. Then use `docker-compose up -d`.

## Check ccloudexporter
Go to http://localhost:2112/metrics. you will see metric of your Kafka cluster similar to matric-example.txt file.

## Prerequisite
1. You need Docker and docker-compose in your local
2. API Key in Confluent Cloud
3. Datadog API key

## How to run

Make sure you are on bash terminal e.g. GIT BASH. `export` is not work in powershell

```
export CCLOUD_API_KEY=<your API KEY>
export CCLOUD_API_SECRET=<your API SECRET>
export CCLOUD_CLUSTER=<your cluster>
export DD_API_KEY=<Datadog API KEY>
docker-compose up -d
```