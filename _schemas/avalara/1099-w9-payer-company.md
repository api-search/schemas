---
description: PayerCompany schema from Avalara API
layout: schema
name: PayerCompany
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: Employer Identification Number
  name: ein
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: contactName
  type: string
- description: ''
  name: contactPhone
  type: string
- description: ''
  name: contactEmail
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/1099-w9-payer-company-schema.json
slug: 1099-w9-payer-company
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-payer-company-schema.json\",\n  \"title\": \"PayerCompany\",\n  \"description\": \"PayerCompany schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"ein\": {\n      \"type\": \"string\",\n      \"description\": \"Employer Identification Number\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"contactName\": {\n      \"type\": \"string\"\n    },\n    \"contactPhone\"\
  : {\n      \"type\": \"string\"\n    },\n    \"contactEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-payer-company-schema.json
tags:
- Taxes
title: PayerCompany
---
