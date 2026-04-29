---
description: ErrorResponse schema from Aramark Marko API
layout: schema
name: ErrorResponse
properties_list:
- description: Error message
  name: message
  type: string
- description: Error code
  name: code
  type: integer
provider_name: Aramark
provider_slug: aramark
schema_file: json-schema/marko-api-error-response-schema.json
slug: marko-api-error-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\",\n      \"example\": \"Unauthorized\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"Error code\",\n      \"example\": 401\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"ErrorResponse schema from Aramark Marko API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-error-response-schema.json
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
title: ErrorResponse
---
