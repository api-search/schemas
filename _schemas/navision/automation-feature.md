---
description: ''
layout: schema
name: Feature
properties_list:
- description: The feature ID
  name: id
  type: string
- description: The feature display name
  name: displayName
  type: string
- description: The feature description
  name: description
  type: string
- description: Whether the feature is enabled
  name: enabled
  type: boolean
- description: URL to documentation about the feature
  name: learnMoreUrl
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/automation-feature-schema.json
slug: automation-feature
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Feature\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The feature ID\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The feature display name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The feature description\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the feature is enabled\"\n    },\n    \"learnMoreUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to documentation about the feature\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/automation-feature-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: Feature
---
