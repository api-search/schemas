---
description: Deployment information.
layout: schema
name: DeploymentExtended
properties_list:
- description: The ID of the deployment.
  name: id
  type: string
- description: The name of the deployment.
  name: name
  type: string
- description: The type of the deployment.
  name: type
  type: string
- description: The location of the deployment.
  name: location
  type: string
- description: Deployment tags.
  name: tags
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-deployment-extended-schema.json
slug: azure-resource-manager-deployment-extended
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentExtended\",\n  \"type\": \"object\",\n  \"description\": \"Deployment information.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the deployment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the deployment.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the deployment.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the deployment.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Deployment tags.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-deployment-extended-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: DeploymentExtended
---
