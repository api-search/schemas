---
description: API error response
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: errorCode
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: requestId
  type: string
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/errorresponse-schema.json
slug: errorresponse
source_filename: errorresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/errorresponse-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"API error response\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"requestId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/errorresponse-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: ErrorResponse
---
