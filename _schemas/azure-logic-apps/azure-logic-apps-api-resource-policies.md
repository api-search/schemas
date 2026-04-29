---
description: The API resource policies.
layout: schema
name: ApiResourcePolicies
properties_list:
- description: The API level only policies XML as embedded content.
  name: content
  type: string
- description: The content link to the policies.
  name: contentLink
  type: string
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-api-resource-policies-schema.json
slug: azure-logic-apps-api-resource-policies
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-resource-policies-schema.json\",\n  \"title\": \"ApiResourcePolicies\",\n  \"description\": \"The API resource policies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"description\": \"The API level only policies XML as embedded content.\",\n      \"type\": \"string\"\n    },\n    \"contentLink\": {\n      \"description\": \"The content link to the policies.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-api-resource-policies-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ApiResourcePolicies
---
