---
description: The container probe, for liveness or readiness
layout: schema
name: ContainerProbe
properties_list:
- description: The execution command to probe
  name: exec
  type: object
- description: The failure threshold.
  name: failureThreshold
  type: integer
- description: The Http Get settings to probe
  name: httpGet
  type: object
- description: The initial delay seconds.
  name: initialDelaySeconds
  type: integer
- description: The period seconds.
  name: periodSeconds
  type: integer
- description: The success threshold.
  name: successThreshold
  type: integer
- description: The timeout seconds.
  name: timeoutSeconds
  type: integer
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-probe-schema.json
slug: azure-container-instances-container-probe
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-probe-schema.json\",\n  \"title\": \"ContainerProbe\",\n  \"description\": \"The container probe, for liveness or readiness\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exec\": {\n      \"$ref\": \"#/definitions/ContainerExec\",\n      \"description\": \"The execution command to probe\"\n    },\n    \"failureThreshold\": {\n      \"description\": \"The failure threshold.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"httpGet\": {\n      \"$ref\": \"#/definitions/ContainerHttpGet\",\n      \"description\": \"The Http Get settings to probe\"\n    },\n    \"initialDelaySeconds\": {\n      \"description\": \"The initial delay seconds.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"periodSeconds\"\
  : {\n      \"description\": \"The period seconds.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"successThreshold\": {\n      \"description\": \"The success threshold.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"timeoutSeconds\": {\n      \"description\": \"The timeout seconds.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-probe-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerProbe
---
