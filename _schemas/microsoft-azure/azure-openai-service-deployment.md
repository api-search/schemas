---
description: Describes a model deployment.
layout: schema
name: Deployment
properties_list:
- description: The deployment identifier.
  name: id
  type: string
- description: ''
  name: object
  type: string
- description: The Unix timestamp when the deployment was created.
  name: created_at
  type: integer
- description: The Unix timestamp when the deployment was last updated.
  name: updated_at
  type: integer
- description: The model identifier deployed.
  name: model
  type: string
- description: The owner of the deployment.
  name: owner
  type: string
- description: The current status of the deployment.
  name: status
  type: string
- description: The deployment scale settings.
  name: scale_settings
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-deployment-schema.json
slug: azure-openai-service-deployment
source_filename: azure-openai-service-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Deployment\",\n  \"type\": \"object\",\n  \"description\": \"Describes a model deployment.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The deployment identifier.\"\n    },\n    \"object\": {\n      \"type\": \"string\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"The Unix timestamp when the deployment was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"integer\",\n      \"description\": \"The Unix timestamp when the deployment was last updated.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model identifier deployed.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The owner of the deployment.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the deployment.\"\n\
  \    },\n    \"scale_settings\": {\n      \"type\": \"object\",\n      \"description\": \"The deployment scale settings.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-deployment-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Deployment
---
