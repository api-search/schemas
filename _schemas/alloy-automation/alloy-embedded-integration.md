---
description: An available integration in the Alloy catalog
layout: schema
name: Integration
properties_list:
- description: Unique identifier for the integration
  name: integrationId
  type: string
- description: Display name of the integration
  name: name
  type: string
- description: Integration category
  name: category
  type: string
- description: URL to the integration icon
  name: iconUrl
  type: string
- description: Whether the integration is installed for the user
  name: installed
  type: boolean
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-integration-schema.json
slug: alloy-embedded-integration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-integration-schema.json\",\n  \"title\": \"Integration\",\n  \"type\": \"object\",\n  \"description\": \"An available integration in the Alloy catalog\",\n  \"properties\": {\n    \"integrationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the integration\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the integration\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Integration category\"\n    },\n    \"iconUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the integration icon\"\n    },\n    \"installed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the integration is installed for the user\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-integration-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: Integration
---
