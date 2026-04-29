---
description: Represents spend data for an application tracked in the Productiv platform.
layout: schema
name: SpendData
properties_list:
- description: The spend amount.
  name: amount
  type: number
- description: The currency code (e.g., USD).
  name: currency
  type: string
- description: The date of the spend.
  name: date
  type: string
- description: A description of the spend.
  name: description
  type: string
provider_name: Productiv
provider_slug: productiv
schema_file: json-schema/spend-data.json
slug: spend-data
source_json: "{\n  \"$id\": \"spend-data.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SpendData\",\n  \"description\": \"Represents spend data for an application tracked in the Productiv platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"The spend amount.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The currency code (e.g., USD).\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of the spend.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the spend.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/json-schema/spend-data.json
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
title: SpendData
---
