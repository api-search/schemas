---
description: ''
layout: schema
name: Connection
properties_list:
- description: Connection ID
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: institution
  type: object
- description: ''
  name: lastUpdated
  type: string
provider_name: Basiq
provider_slug: basiq
schema_file: json-schema/connection.json
slug: connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/connection.json\",\n  \"title\": \"Connection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Connection ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"pending\",\n        \"failed\",\n        \"disconnected\"\n      ]\n    },\n    \"institution\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/connection.json
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
title: Connection
---
