---
description: The list of managed API operations.
layout: schema
name: ApiOperationListResult
properties_list:
- description: The URL to get the next set of results.
  name: nextLink
  type: string
- description: The api operation definitions for an API.
  name: value
  type: array
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-api-operation-list-result-schema.json
slug: azure-logic-apps-api-operation-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-operation-list-result-schema.json\",\n  \"title\": \"ApiOperationListResult\",\n  \"description\": \"The list of managed API operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URL to get the next set of results.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The api operation definitions for an API.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ApiOperation\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-operation-list-result-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiOperationListResult
---
