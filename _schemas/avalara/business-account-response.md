---
description: AccountResponse schema from Avalara API
layout: schema
name: AccountResponse
properties_list:
- description: ''
  name: accountId
  type: string
- description: ''
  name: accountNumber
  type: string
- description: ''
  name: companyName
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: createdDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/business-account-response-schema.json
slug: business-account-response
source_filename: business-account-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/business-account-response-schema.json\",\n  \"title\": \"AccountResponse\",\n  \"description\": \"AccountResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\"\n    },\n    \"companyName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Inactive\",\n        \"Pending\"\n      ]\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/business-account-response-schema.json
tags:
- Taxes
title: AccountResponse
---
