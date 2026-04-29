---
description: Properties of Cognitive Services account deployment.
layout: schema
name: DeploymentProperties
properties_list:
- description: The provisioning state of the deployment.
  name: provisioningState
  type: string
- description: The deployment scale settings.
  name: scaleSettings
  type: object
- description: The rate limits for the deployment.
  name: rateLimits
  type: array
- description: The capabilities of the deployment.
  name: capabilities
  type: object
- description: Deployment model version upgrade option.
  name: versionUpgradeOption
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cognitive-services-deployment-properties-schema.json
slug: azure-cognitive-services-deployment-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of Cognitive Services account deployment.\",\n  \"properties\": {\n    \"provisioningState\": {\n      \"type\": \"string\",\n      \"description\": \"The provisioning state of the deployment.\"\n    },\n    \"scaleSettings\": {\n      \"type\": \"object\",\n      \"description\": \"The deployment scale settings.\"\n    },\n    \"rateLimits\": {\n      \"type\": \"array\",\n      \"description\": \"The rate limits for the deployment.\"\n    },\n    \"capabilities\": {\n      \"type\": \"object\",\n      \"description\": \"The capabilities of the deployment.\"\n    },\n    \"versionUpgradeOption\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment model version upgrade option.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cognitive-services-deployment-properties-schema.json
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
