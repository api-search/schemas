---
description: Deployment operation parameters.
layout: schema
name: Deployment
properties_list:
- description: The location to store the deployment data.
  name: location
  type: string
- description: Deployment tags.
  name: tags
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-deployment-schema.json
slug: azure-resource-manager-deployment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Deployment\",\n  \"type\": \"object\",\n  \"description\": \"Deployment operation parameters.\",\n  \"properties\": {\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The location to store the deployment data.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Deployment tags.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-deployment-schema.json
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
