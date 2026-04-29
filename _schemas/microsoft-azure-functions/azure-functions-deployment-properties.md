---
description: Deployment resource specific properties
layout: schema
name: DeploymentProperties
properties_list:
- description: Deployment status.
  name: status
  type: integer
- description: Details about deployment status.
  name: message
  type: string
- description: Who authored the deployment.
  name: author
  type: string
- description: Who performed the deployment.
  name: deployer
  type: string
- description: Author email.
  name: author_email
  type: string
- description: Start time.
  name: start_time
  type: string
- description: End time.
  name: end_time
  type: string
- description: True if deployment is currently active, false if completed and null if not started.
  name: active
  type: boolean
- description: Details on deployment.
  name: details
  type: string
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-deployment-properties-schema.json
slug: azure-functions-deployment-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-deployment-properties-schema.json\",\n  \"title\": \"DeploymentProperties\",\n  \"description\": \"Deployment resource specific properties\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Deployment status.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Details about deployment status.\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"Who authored the deployment.\"\n    },\n    \"deployer\": {\n      \"type\": \"string\",\n      \"description\": \"Who performed the deployment.\"\n    },\n    \"author_email\": {\n      \"type\": \"string\",\n      \"description\": \"Author email.\",\n      \"x-ms-client-name\"\
  : \"authorEmail\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time.\",\n      \"x-ms-client-name\": \"startTime\"\n    },\n    \"end_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"End time.\",\n      \"x-ms-client-name\": \"endTime\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if deployment is currently active, false if completed and null if not started.\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Details on deployment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-deployment-properties-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: DeploymentProperties
---
