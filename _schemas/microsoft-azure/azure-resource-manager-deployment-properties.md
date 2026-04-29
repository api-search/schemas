---
description: Deployment properties.
layout: schema
name: DeploymentProperties
properties_list:
- description: The template content. Use this element when you want to pass the template syntax directly in the request rather than link to an existing template.
  name: template
  type: object
- description: Name and value pairs that define the deployment parameters.
  name: parameters
  type: object
- description: The mode that is used to deploy resources.
  name: mode
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-deployment-properties-schema.json
slug: azure-resource-manager-deployment-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentProperties\",\n  \"type\": \"object\",\n  \"description\": \"Deployment properties.\",\n  \"properties\": {\n    \"template\": {\n      \"type\": \"object\",\n      \"description\": \"The template content. Use this element when you want to pass the template syntax directly in the request rather than link to an existing template.\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Name and value pairs that define the deployment parameters.\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"The mode that is used to deploy resources.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-deployment-properties-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: DeploymentProperties
---
