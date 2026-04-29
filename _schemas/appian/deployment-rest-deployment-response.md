---
description: Response returned when a deployment operation is successfully initiated. Contains the UUID for tracking the deployment and its current status.
layout: schema
name: DeploymentResponse
properties_list:
- description: Unique identifier for the deployment operation. Use this UUID to retrieve deployment results and logs.
  name: uuid
  type: string
- description: URL endpoint for retrieving the deployment details and results.
  name: url
  type: string
- description: ''
  name: status
  type: object
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-deployment-response-schema.json
slug: deployment-rest-deployment-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-deployment-response-schema.json\",\n  \"title\": \"DeploymentResponse\",\n  \"description\": \"Response returned when a deployment operation is successfully initiated. Contains the UUID for tracking the deployment and its current status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the deployment operation. Use this UUID to retrieve deployment results and logs.\",\n      \"example\": \"d243b14c-3ba5-41c3-9f51-76da51beb8f5\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL endpoint for retrieving the deployment details and results.\",\n      \"example\": \"https://mysite.appiancloud.com/suite/deployment-management/v2/deployments/d243b14c-3ba5-41c3-9f51-76da51beb8f5/\"\
  \n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/DeploymentStatus\"\n    }\n  },\n  \"required\": [\n    \"uuid\",\n    \"url\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-deployment-response-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: DeploymentResponse
---
