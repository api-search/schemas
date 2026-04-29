---
description: The container instance state.
layout: schema
name: ContainerState
properties_list:
- description: The human-readable status of the container instance state.
  name: detailStatus
  type: string
- description: The container instance exit codes correspond to those from the `docker run` command.
  name: exitCode
  type: integer
- description: The date-time when the container instance state finished.
  name: finishTime
  type: string
- description: The date-time when the container instance state started.
  name: startTime
  type: string
- description: The state of the container instance.
  name: state
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-state-schema.json
slug: azure-container-instances-container-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-state-schema.json\",\n  \"title\": \"ContainerState\",\n  \"description\": \"The container instance state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detailStatus\": {\n      \"description\": \"The human-readable status of the container instance state.\",\n      \"type\": \"string\"\n    },\n    \"exitCode\": {\n      \"description\": \"The container instance exit codes correspond to those from the `docker run` command.\",\n      \"type\": \"integer\"\n    },\n    \"finishTime\": {\n      \"description\": \"The date-time when the container instance state finished.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"description\": \"The date-time when the container instance state started.\",\n\
  \      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"description\": \"The state of the container instance.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-state-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerState
---
