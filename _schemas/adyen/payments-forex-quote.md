---
description: ForexQuote schema from Adyen API
layout: schema
name: ForexQuote
properties_list:
- description: The account name.
  name: account
  type: string
- description: The account type.
  name: accountType
  type: string
- description: The base amount.
  name: baseAmount
  type: object
- description: The base points.
  name: basePoints
  type: integer
- description: The buy rate.
  name: buy
  type: object
- description: The interbank amount.
  name: interbank
  type: object
- description: The reference assigned to the forex quote request.
  name: reference
  type: string
- description: The sell rate.
  name: sell
  type: object
- description: The signature to validate the integrity.
  name: signature
  type: string
- description: The source of the forex quote.
  name: source
  type: string
- description: The type of forex.
  name: type
  type: string
- description: The date until which the forex quote is valid.
  name: validTill
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-forex-quote-schema.json
slug: payments-forex-quote
source_filename: payments-forex-quote-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-forex-quote-schema.json\",\n  \"title\": \"ForexQuote\",\n  \"description\": \"ForexQuote schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account\": {\n      \"description\": \"The account name.\",\n      \"type\": \"string\"\n    },\n    \"accountType\": {\n      \"description\": \"The account type.\",\n      \"type\": \"string\"\n    },\n    \"baseAmount\": {\n      \"description\": \"The base amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"basePoints\": {\n      \"description\": \"The base points.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"buy\": {\n      \"description\": \"The buy rate.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"interbank\": {\n      \"description\": \"The interbank amount.\"\
  ,\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"reference\": {\n      \"description\": \"The reference assigned to the forex quote request.\",\n      \"type\": \"string\"\n    },\n    \"sell\": {\n      \"description\": \"The sell rate.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"signature\": {\n      \"description\": \"The signature to validate the integrity.\",\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"description\": \"The source of the forex quote.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of forex.\",\n      \"type\": \"string\"\n    },\n    \"validTill\": {\n      \"description\": \"The date until which the forex quote is valid.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"validTill\",\n    \"basePoints\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-forex-quote-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ForexQuote
---
