---
description: ContainerApp schema from Azure Container Apps API
layout: schema
name: ContainerApp
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
  name: location
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: identity
  type: object
- description: ''
  name: properties
  type: object
provider_name: Azure Container Apps
provider_slug: azure-container-apps
schema_file: json-schema/azure-container-apps-container-app-schema.json
slug: azure-container-apps-container-app
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-container-app-schema.json\",\n  \"title\": \"ContainerApp\",\n  \"description\": \"ContainerApp schema from Azure Container Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"identity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"None\",\n     \
  \       \"SystemAssigned\",\n            \"UserAssigned\",\n            \"SystemAssigned,UserAssigned\"\n          ]\n        },\n        \"principalId\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"tenantId\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"userAssignedIdentities\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"principalId\": {\n                \"type\": \"string\",\n                \"readOnly\": true\n              },\n              \"clientId\": {\n                \"type\": \"string\",\n                \"readOnly\": true\n              }\n            }\n          }\n        }\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n        \
  \  \"enum\": [\n            \"InProgress\",\n            \"Succeeded\",\n            \"Failed\",\n            \"Canceled\",\n            \"Deleting\"\n          ]\n        },\n        \"managedEnvironmentId\": {\n          \"type\": \"string\",\n          \"description\": \"Resource ID of the Container App's environment.\"\n        },\n        \"environmentId\": {\n          \"type\": \"string\",\n          \"description\": \"Resource ID of the environment.\"\n        },\n        \"workloadProfileName\": {\n          \"type\": \"string\"\n        },\n        \"latestRevisionName\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"latestReadyRevisionName\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"latestRevisionFqdn\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"customDomainVerificationId\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n \
  \       },\n        \"outboundIpAddresses\": {\n          \"type\": \"array\",\n          \"readOnly\": true,\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"eventStreamEndpoint\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"configuration\": {\n          \"$ref\": \"#/components/schemas/Configuration\"\n        },\n        \"template\": {\n          \"$ref\": \"#/components/schemas/Template\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-container-app-schema.json
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: ContainerApp
---
