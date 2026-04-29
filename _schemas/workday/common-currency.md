---
description: ''
layout: schema
name: Currency
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The ISO 4217 currency code.
  name: currencyCode
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: numericCode
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/common-currency-schema.json
slug: common-currency
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Currency\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 4217 currency code.\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"numericCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/common-currency-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Currency
---
