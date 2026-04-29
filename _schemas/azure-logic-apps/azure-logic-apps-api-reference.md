---
description: The Api reference.
layout: schema
name: ApiReference
properties_list:
- description: The brand color of the api.
  name: brandColor
  type: string
- description: The tier.
  name: category
  type: object
- description: The description of the api.
  name: description
  type: string
- description: The display name of the api.
  name: displayName
  type: string
- description: The icon uri of the api.
  name: iconUri
  type: string
- description: The integration service environment reference.
  name: integrationServiceEnvironment
  type: object
- description: The swagger of the api.
  name: swagger
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-api-reference-schema.json
slug: azure-logic-apps-api-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-reference-schema.json\",\n  \"title\": \"ApiReference\",\n  \"description\": \"The Api reference.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brandColor\": {\n      \"description\": \"The brand color of the api.\",\n      \"type\": \"string\"\n    },\n    \"category\": {\n      \"$ref\": \"#/definitions/ApiTier\",\n      \"description\": \"The tier.\"\n    },\n    \"description\": {\n      \"description\": \"The description of the api.\",\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"description\": \"The display name of the api.\",\n      \"type\": \"string\"\n    },\n    \"iconUri\": {\n      \"description\": \"The icon uri of the api.\",\n      \"type\": \"string\"\n    },\n    \"integrationServiceEnvironment\": {\n      \"$ref\": \"#/definitions/ResourceReference\"\
  ,\n      \"description\": \"The integration service environment reference.\"\n    },\n    \"swagger\": {\n      \"$ref\": \"#/definitions/Object\",\n      \"description\": \"The swagger of the api.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-reference-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiReference
---
