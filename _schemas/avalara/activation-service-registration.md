---
description: Registration schema from Avalara API
layout: schema
name: Registration
properties_list:
- description: ''
  name: registrationId
  type: string
- description: ''
  name: partnerId
  type: string
- description: ''
  name: companyName
  type: string
- description: ''
  name: status
  type: string
- description: Avalara product registered for
  name: product
  type: string
- description: ''
  name: accountId
  type: string
- description: ''
  name: activationDate
  type: string
- description: ''
  name: expirationDate
  type: string
- description: ''
  name: createdDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/activation-service-registration-schema.json
slug: activation-service-registration
source_filename: activation-service-registration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/activation-service-registration-schema.json\",\n  \"title\": \"Registration\",\n  \"description\": \"Registration schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"registrationId\": {\n      \"type\": \"string\"\n    },\n    \"partnerId\": {\n      \"type\": \"string\"\n    },\n    \"companyName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pending\",\n        \"Active\",\n        \"Expired\",\n        \"Cancelled\"\n      ]\n    },\n    \"product\": {\n      \"type\": \"string\",\n      \"description\": \"Avalara product registered for\"\n    },\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"activationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"expirationDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/activation-service-registration-schema.json
tags:
- Taxes
title: Registration
---
