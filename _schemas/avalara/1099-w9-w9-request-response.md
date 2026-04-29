---
description: W9RequestResponse schema from Avalara API
layout: schema
name: W9RequestResponse
properties_list:
- description: ''
  name: requestId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: payeeEmail
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: expirationDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/1099-w9-w9-request-response-schema.json
slug: 1099-w9-w9-request-response
source_filename: 1099-w9-w9-request-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-w9-request-response-schema.json\",\n  \"title\": \"W9RequestResponse\",\n  \"description\": \"W9RequestResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"payeeEmail\": {\n      \"type\": \"string\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-w9-request-response-schema.json
tags:
- Taxes
title: W9RequestResponse
---
