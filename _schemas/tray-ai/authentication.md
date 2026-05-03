---
description: A third-party service authentication used by Tray.ai connectors to access external services.
layout: schema
name: Tray.ai Authentication
properties_list:
- description: Unique authentication identifier
  name: id
  type: string
- description: Display name of the authentication
  name: name
  type: string
- description: The service environment against which this authentication was created
  name: serviceEnvironmentId
  type: string
- description: The third-party service this authentication is for
  name: service
  type: object
- description: The service environment instance
  name: serviceEnvironment
  type: object
- description: OAuth scopes associated with this authentication
  name: scopes
  type: array
- description: Timestamp when the authentication was created
  name: createdAt
  type: string
provider_name: Tray.ai
provider_slug: tray-ai
schema_file: json-schema/authentication.json
slug: authentication
source_filename: authentication.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/authentication.json\",\n  \"title\": \"Tray.ai Authentication\",\n  \"description\": \"A third-party service authentication used by Tray.ai connectors to access external services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique authentication identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the authentication\"\n    },\n    \"serviceEnvironmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The service environment against which this authentication was created\"\n    },\n    \"service\": {\n      \"type\": \"object\",\n      \"description\": \"The third-party service this authentication is for\",\n      \"properties\": {\n        \"id\": {\n          \"type\":\
  \ \"string\",\n          \"description\": \"Service identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Service display name\"\n        },\n        \"icon\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the service icon\"\n        }\n      }\n    },\n    \"serviceEnvironment\": {\n      \"type\": \"object\",\n      \"description\": \"The service environment instance\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Service environment identifier\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Service environment display name\"\n        }\n      }\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"description\": \"OAuth scopes associated with this authentication\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createdAt\":\
  \ {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the authentication was created\"\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/authentication.json
tags:
- Automation
- Integration
- iPaaS
title: Tray.ai Authentication
---
