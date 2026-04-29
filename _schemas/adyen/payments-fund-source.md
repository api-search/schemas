---
description: FundSource schema from Adyen API
layout: schema
name: FundSource
properties_list:
- description: A map of name-value pairs for passing additional or industry-specific data.
  name: additionalData
  type: object
- description: The address where to send the invoice.
  name: billingAddress
  type: object
- description: Credit card data. Optional if `shopperReference` and `selectedRecurringDetailReference` are provided.
  name: card
  type: object
- description: Email address of the person.
  name: shopperEmail
  type: string
- description: Name of the person.
  name: shopperName
  type: object
- description: Phone number of the person
  name: telephoneNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-fund-source-schema.json
slug: payments-fund-source
source_filename: payments-fund-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-fund-source-schema.json\",\n  \"title\": \"FundSource\",\n  \"description\": \"FundSource schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A map of name-value pairs for passing additional or industry-specific data.\",\n      \"type\": \"object\"\n    },\n    \"billingAddress\": {\n      \"description\": \"The address where to send the invoice.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"card\": {\n      \"description\": \"Credit card data.\\n\\nOptional if `shopperReference` and `selectedRecurringDetailReference` are provided.\",\n      \"$ref\": \"#/components/schemas/Card\"\n    },\n    \"shopperEmail\": {\n      \"description\":\
  \ \"Email address of the person.\",\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"description\": \"Name of the person.\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"telephoneNumber\": {\n      \"description\": \"Phone number of the person\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-fund-source-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: FundSource
---
