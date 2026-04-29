---
description: W9Request schema from Avalara API
layout: schema
name: W9Request
properties_list:
- description: ''
  name: payeeEmail
  type: string
- description: ''
  name: payeeName
  type: string
- description: ''
  name: companyId
  type: string
- description: ''
  name: expirationDays
  type: integer
- description: ''
  name: message
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/1099-w9-w9-request-schema.json
slug: 1099-w9-w9-request
source_filename: 1099-w9-w9-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-w9-request-schema.json\",\n  \"title\": \"W9Request\",\n  \"description\": \"W9Request schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"payeeEmail\",\n    \"payeeName\"\n  ],\n  \"properties\": {\n    \"payeeEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    },\n    \"payeeName\": {\n      \"type\": \"string\"\n    },\n    \"companyId\": {\n      \"type\": \"string\"\n    },\n    \"expirationDays\": {\n      \"type\": \"integer\",\n      \"default\": 30\n    },\n    \"message\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-w9-request-schema.json
tags:
- Taxes
title: W9Request
---
