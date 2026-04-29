---
description: Party schema from Avalara API
layout: schema
name: Party
properties_list:
- description: ''
  name: name
  type: string
- description: Tax identification number
  name: identifier
  type: string
- description: Identifier scheme (e.g., VAT)
  name: identifierScheme
  type: string
- description: ''
  name: address
  type: object
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-party-schema.json
slug: e-invoicing-party
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-party-schema.json\",\n  \"title\": \"Party\",\n  \"description\": \"Party schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Tax identification number\"\n    },\n    \"identifierScheme\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier scheme (e.g., VAT)\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"region\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"countryCode\": {\n\
  \          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-party-schema.json
tags:
- Taxes
title: Party
---
