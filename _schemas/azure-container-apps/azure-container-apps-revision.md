---
description: Revision schema from Azure Container Apps API
layout: schema
name: Revision
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Container Apps
provider_slug: azure-container-apps
schema_file: json-schema/azure-container-apps-revision-schema.json
slug: azure-container-apps-revision
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-revision-schema.json\",\n  \"title\": \"Revision\",\n  \"description\": \"Revision schema from Azure Container Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"createdTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"readOnly\": true\n        },\n        \"lastActiveTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"readOnly\": true\n        },\n        \"fqdn\"\
  : {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"template\": {\n          \"$ref\": \"#/components/schemas/Template\"\n        },\n        \"active\": {\n          \"type\": \"boolean\",\n          \"readOnly\": true\n        },\n        \"replicas\": {\n          \"type\": \"integer\",\n          \"readOnly\": true\n        },\n        \"trafficWeight\": {\n          \"type\": \"integer\",\n          \"readOnly\": true\n        },\n        \"provisioningError\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"healthState\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"enum\": [\n            \"Healthy\",\n            \"Unhealthy\",\n            \"None\"\n          ]\n        },\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"enum\": [\n            \"Provisioning\",\n            \"Provisioned\",\n            \"\
  Failed\",\n            \"Deprovisioning\",\n            \"Deprovisioned\"\n          ]\n        },\n        \"runningState\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"enum\": [\n            \"Running\",\n            \"Processing\",\n            \"Stopped\",\n            \"Degraded\",\n            \"Failed\",\n            \"Unknown\"\n          ]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-revision-schema.json
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: Revision
---
