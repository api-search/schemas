---
description: JobExecutionTemplate schema from Azure Container Apps API
layout: schema
name: JobExecutionTemplate
properties_list:
- description: ''
  name: containers
  type: array
- description: ''
  name: initContainers
  type: array
provider_name: Azure Container Apps
provider_slug: azure-container-apps
schema_file: json-schema/azure-container-apps-job-execution-template-schema.json
slug: azure-container-apps-job-execution-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-job-execution-template-schema.json\",\n  \"title\": \"JobExecutionTemplate\",\n  \"description\": \"JobExecutionTemplate schema from Azure Container Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"containers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Container\"\n      }\n    },\n    \"initContainers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Container\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-job-execution-template-schema.json
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: JobExecutionTemplate
---
