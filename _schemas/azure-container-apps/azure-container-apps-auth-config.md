---
description: AuthConfig schema from Azure Container Apps API
layout: schema
name: AuthConfig
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
schema_file: json-schema/azure-container-apps-auth-config-schema.json
slug: azure-container-apps-auth-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-auth-config-schema.json\",\n  \"title\": \"AuthConfig\",\n  \"description\": \"AuthConfig schema from Azure Container Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"platform\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\"\n            },\n            \"runtimeVersion\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"globalValidation\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"unauthenticatedClientAction\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"RedirectToLoginPage\",\n                \"AllowAnonymous\",\n                \"Return401\",\n                \"Return403\"\n              ]\n            },\n            \"redirectToProvider\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"identityProviders\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"azureActiveDirectory\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"enabled\": {\n                  \"type\": \"boolean\"\n                },\n                \"registration\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"openIdIssuer\": {\n                      \"type\": \"string\"\n                    },\n      \
  \              \"clientId\": {\n                      \"type\": \"string\"\n                    },\n                    \"clientSecretSettingName\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-auth-config-schema.json
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: AuthConfig
---
