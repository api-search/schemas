---
description: JobExecution schema from Azure Container Apps API
layout: schema
name: JobExecution
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Container Apps
provider_slug: azure-container-apps
schema_file: json-schema/azure-container-apps-job-execution-schema.json
slug: azure-container-apps-job-execution
source_filename: azure-container-apps-job-execution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-job-execution-schema.json\",\n  \"title\": \"JobExecution\",\n  \"description\": \"JobExecution schema from Azure Container Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"enum\": [\n            \"Running\",\n            \"Processing\",\n            \"Stopped\",\n            \"Degraded\",\n            \"Failed\",\n            \"Unknown\",\n            \"Succeeded\"\n          ]\n        },\n        \"startTime\": {\n          \"type\": \"\
  string\",\n          \"format\": \"date-time\",\n          \"readOnly\": true\n        },\n        \"endTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"readOnly\": true\n        },\n        \"template\": {\n          \"$ref\": \"#/components/schemas/JobExecutionTemplate\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-job-execution-schema.json
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: JobExecution
---
