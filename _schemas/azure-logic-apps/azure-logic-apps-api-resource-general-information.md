---
description: The API general information.
layout: schema
name: ApiResourceGeneralInformation
properties_list:
- description: The description.
  name: description
  type: string
- description: The display name.
  name: displayName
  type: string
- description: The icon url.
  name: iconUrl
  type: string
- description: The release tag.
  name: releaseTag
  type: string
- description: The terms of use url.
  name: termsOfUseUrl
  type: string
- description: The tier.
  name: tier
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-api-resource-general-information-schema.json
slug: azure-logic-apps-api-resource-general-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-resource-general-information-schema.json\",\n  \"title\": \"ApiResourceGeneralInformation\",\n  \"description\": \"The API general information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"The description.\",\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"description\": \"The display name.\",\n      \"type\": \"string\"\n    },\n    \"iconUrl\": {\n      \"description\": \"The icon url.\",\n      \"type\": \"string\"\n    },\n    \"releaseTag\": {\n      \"description\": \"The release tag.\",\n      \"type\": \"string\"\n    },\n    \"termsOfUseUrl\": {\n      \"description\": \"The terms of use url.\",\n      \"type\": \"string\"\n    },\n    \"tier\": {\n      \"$ref\": \"#/definitions/ApiTier\",\n     \
  \ \"description\": \"The tier.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-resource-general-information-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiResourceGeneralInformation
---
