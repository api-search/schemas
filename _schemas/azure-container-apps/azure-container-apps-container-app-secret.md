---
description: ContainerAppSecret schema from Azure Container Apps API
layout: schema
name: ContainerAppSecret
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: value
  type: string
provider_name: Azure Container Apps
provider_slug: azure-container-apps
schema_file: json-schema/azure-container-apps-container-app-secret-schema.json
slug: azure-container-apps-container-app-secret
source_filename: azure-container-apps-container-app-secret-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-container-app-secret-schema.json\",\n  \"title\": \"ContainerAppSecret\",\n  \"description\": \"ContainerAppSecret schema from Azure Container Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-container-app-secret-schema.json
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: ContainerAppSecret
---
