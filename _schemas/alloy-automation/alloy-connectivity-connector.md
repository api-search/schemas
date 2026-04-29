---
description: A third-party application connector available in Alloy
layout: schema
name: Connector
properties_list:
- description: Unique identifier for the connector
  name: connectorId
  type: string
- description: Display name of the connector
  name: name
  type: string
- description: Connector category
  name: category
  type: string
- description: URL to the connector icon
  name: iconUrl
  type: string
- description: Number of available actions for this connector
  name: actionCount
  type: integer
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-connector-schema.json
slug: alloy-connectivity-connector
source_filename: alloy-connectivity-connector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-connector-schema.json\",\n  \"title\": \"Connector\",\n  \"type\": \"object\",\n  \"description\": \"A third-party application connector available in Alloy\",\n  \"properties\": {\n    \"connectorId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the connector\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the connector\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Connector category\"\n    },\n    \"iconUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the connector icon\"\n    },\n    \"actionCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of available actions for this connector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-connector-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: Connector
---
