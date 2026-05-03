---
description: A Tray.ai connector that exposes third-party API operations for integration workflows.
layout: schema
name: Tray.ai Connector
properties_list:
- description: The connector name identifier (e.g., salesforce, slack)
  name: name
  type: string
- description: Display name of the connector
  name: title
  type: string
- description: Description of the connector and its capabilities
  name: description
  type: string
- description: URL to the connector icon
  name: icon
  type: string
- description: Available versions of the connector
  name: versions
  type: array
provider_name: Tray.ai
provider_slug: tray-ai
schema_file: json-schema/connector.json
slug: connector
source_filename: connector.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/connector.json\",\n  \"title\": \"Tray.ai Connector\",\n  \"description\": \"A Tray.ai connector that exposes third-party API operations for integration workflows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The connector name identifier (e.g., salesforce, slack)\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the connector\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the connector and its capabilities\"\n    },\n    \"icon\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the connector icon\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"Available\
  \ versions of the connector\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"version\": {\n            \"type\": \"string\",\n            \"description\": \"Version identifier\"\n          },\n          \"isLatest\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this is the latest version\"\n          },\n          \"operations\": {\n            \"type\": \"array\",\n            \"description\": \"Operations available in this version\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"description\": \"Operation name identifier\"\n                },\n                \"title\": {\n                  \"type\": \"string\",\n                  \"description\": \"Display name of the operation\"\n                },\n                \"description\": {\n                  \"type\": \"string\"\
  ,\n                  \"description\": \"Description of what the operation does\"\n                },\n                \"inputSchema\": {\n                  \"type\": \"object\",\n                  \"description\": \"JSON Schema defining the operation input\"\n                },\n                \"outputSchema\": {\n                  \"type\": \"object\",\n                  \"description\": \"JSON Schema defining the operation output\"\n                }\n              },\n              \"required\": [\"name\"]\n            }\n          }\n        },\n        \"required\": [\"version\"]\n      }\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/connector.json
tags:
- Automation
- Integration
- iPaaS
title: Tray.ai Connector
---
