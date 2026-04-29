---
description: Deployment properties with additional details.
layout: schema
name: DeploymentPropertiesExtended
properties_list:
- description: Denotes the state of provisioning.
  name: provisioningState
  type: string
- description: The correlation ID of the deployment.
  name: correlationId
  type: string
- description: The timestamp of the template deployment.
  name: timestamp
  type: string
- description: The duration of the template deployment.
  name: duration
  type: string
- description: Key/value pairs that represent deployment output.
  name: outputs
  type: object
- description: The deployment mode.
  name: mode
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-deployment-properties-extended-schema.json
slug: azure-resource-manager-deployment-properties-extended
source_filename: azure-resource-manager-deployment-properties-extended-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentPropertiesExtended\",\n  \"type\": \"object\",\n  \"description\": \"Deployment properties with additional details.\",\n  \"properties\": {\n    \"provisioningState\": {\n      \"type\": \"string\",\n      \"description\": \"Denotes the state of provisioning.\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"The correlation ID of the deployment.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp of the template deployment.\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"The duration of the template deployment.\"\n    },\n    \"outputs\": {\n      \"type\": \"object\",\n      \"description\": \"Key/value pairs that represent deployment output.\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"The deployment mode.\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-deployment-properties-extended-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: DeploymentPropertiesExtended
---
