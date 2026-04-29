---
description: ''
layout: schema
name: Error
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: innerException
  type: object
- description: ''
  name: message
  type: string
- description: ''
  name: typeName
  type: string
- description: ''
  name: typeKey
  type: string
- description: ''
  name: errorCode
  type: integer
- description: ''
  name: eventId
  type: integer
provider_name: Azure DevOps
provider_slug: azure-devops
schema_file: json-schema/azure-devops-work-items-error-schema.json
slug: azure-devops-work-items-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"innerException\": {\n      \"type\": \"object\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"typeName\": {\n      \"type\": \"string\"\n    },\n    \"typeKey\": {\n      \"type\": \"string\"\n    },\n    \"errorCode\": {\n      \"type\": \"integer\"\n    },\n    \"eventId\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/json-schema/azure-devops-work-items-error-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
title: Error
---
