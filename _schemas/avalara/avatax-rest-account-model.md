---
description: AccountModel schema from Avalara API
layout: schema
name: AccountModel
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: effectiveDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: accountStatusId
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: modifiedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-account-model-schema.json
slug: avatax-rest-account-model
source_filename: avatax-rest-account-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-account-model-schema.json\",\n  \"title\": \"AccountModel\",\n  \"description\": \"AccountModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"accountStatusId\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Inactive\",\n        \"Active\",\n        \"Test\",\n        \"New\"\n      ]\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n   \
  \ }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-account-model-schema.json
tags:
- Taxes
title: AccountModel
---
