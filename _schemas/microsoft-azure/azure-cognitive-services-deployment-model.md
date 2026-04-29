---
description: Properties of the deployment model.
layout: schema
name: DeploymentModel
properties_list:
- description: Deployment model format.
  name: format
  type: string
- description: Deployment model name.
  name: name
  type: string
- description: Deployment model version.
  name: version
  type: string
- description: Optional. Deployment model source ARM resource ID.
  name: source
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cognitive-services-deployment-model-schema.json
slug: azure-cognitive-services-deployment-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentModel\",\n  \"type\": \"object\",\n  \"description\": \"Properties of the deployment model.\",\n  \"properties\": {\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment model format.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment model name.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment model version.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Optional. Deployment model source ARM resource ID.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cognitive-services-deployment-model-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: DeploymentModel
---
