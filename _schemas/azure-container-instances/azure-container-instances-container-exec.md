---
description: The container execution command, for liveness or readiness probe
layout: schema
name: ContainerExec
properties_list:
- description: The commands to execute within the container.
  name: command
  type: array
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-exec-schema.json
slug: azure-container-instances-container-exec
source_filename: azure-container-instances-container-exec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-exec-schema.json\",\n  \"title\": \"ContainerExec\",\n  \"description\": \"The container execution command, for liveness or readiness probe\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"command\": {\n      \"description\": \"The commands to execute within the container.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-exec-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerExec
---
