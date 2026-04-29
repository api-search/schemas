---
description: The artifact properties definition.
layout: schema
name: ArtifactProperties
properties_list:
- description: The artifact changed time.
  name: changedTime
  type: string
- description: The artifact creation time.
  name: createdTime
  type: string
- description: ''
  name: metadata
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-artifact-properties-schema.json
slug: azure-logic-apps-artifact-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-artifact-properties-schema.json\",\n  \"title\": \"ArtifactProperties\",\n  \"description\": \"The artifact properties definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"changedTime\": {\n      \"description\": \"The artifact changed time.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"createdTime\": {\n      \"description\": \"The artifact creation time.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-artifact-properties-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: ArtifactProperties
---
