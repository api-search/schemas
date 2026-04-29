---
description: The API deployment parameter metadata.
layout: schema
name: ApiDeploymentParameterMetadata
properties_list:
- description: The description.
  name: description
  type: string
- description: The display name.
  name: displayName
  type: string
- description: Indicates whether its required.
  name: isRequired
  type: boolean
- description: The type.
  name: type
  type: string
- description: The visibility.
  name: visibility
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-api-deployment-parameter-metadata-schema.json
slug: azure-logic-apps-api-deployment-parameter-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-deployment-parameter-metadata-schema.json\",\n  \"title\": \"ApiDeploymentParameterMetadata\",\n  \"description\": \"The API deployment parameter metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"The description.\",\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"description\": \"The display name.\",\n      \"type\": \"string\"\n    },\n    \"isRequired\": {\n      \"description\": \"Indicates whether its required.\",\n      \"type\": \"boolean\"\n    },\n    \"type\": {\n      \"description\": \"The type.\",\n      \"type\": \"string\"\n    },\n    \"visibility\": {\n      \"$ref\": \"#/definitions/ApiDeploymentParameterVisibility\",\n      \"description\": \"The visibility.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-deployment-parameter-metadata-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiDeploymentParameterMetadata
---
