---
description: AmountMinMaxRequirement schema from Adyen API
layout: schema
name: AmountMinMaxRequirement
properties_list:
- description: Specifies the eligible amounts for a particular route.
  name: description
  type: string
- description: Maximum amount.
  name: max
  type: integer
- description: Minimum amount.
  name: min
  type: integer
- description: '**amountMinMaxRequirement**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-amount-min-max-requirement-schema.json
slug: configuration-amount-min-max-requirement
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-amount-min-max-requirement-schema.json\",\n  \"title\": \"AmountMinMaxRequirement\",\n  \"description\": \"AmountMinMaxRequirement schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Specifies the eligible amounts for a particular route.\",\n      \"type\": \"string\"\n    },\n    \"max\": {\n      \"description\": \"Maximum amount.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"min\": {\n      \"description\": \"Minimum amount.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"type\": {\n      \"default\": \"amountMinMaxRequirement\",\n      \"description\": \"**amountMinMaxRequirement**\",\n      \"enum\": [\n        \"amountMinMaxRequirement\"\n      ],\n      \"type\": \"\
  string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-amount-min-max-requirement-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AmountMinMaxRequirement
---
