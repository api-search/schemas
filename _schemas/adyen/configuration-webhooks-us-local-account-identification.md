---
description: USLocalAccountIdentification schema from Adyen API
layout: schema
name: USLocalAccountIdentification
properties_list:
- description: The bank account number, without separators or whitespace.
  name: accountNumber
  type: string
- description: 'The bank account type. Possible values: **checking** or **savings**. Defaults to **checking**.'
  name: accountType
  type: string
- description: The 9-digit [routing number](https://en.wikipedia.org/wiki/ABA_routing_transit_number), without separators or whitespace.
  name: routingNumber
  type: string
- description: '**usLocal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-us-local-account-identification-schema.json
slug: configuration-webhooks-us-local-account-identification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-us-local-account-identification-schema.json\",\n  \"title\": \"USLocalAccountIdentification\",\n  \"description\": \"USLocalAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountNumber\": {\n      \"description\": \"The bank account number, without separators or whitespace.\",\n      \"maxLength\": 18,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"accountType\": {\n      \"default\": \"checking\",\n      \"description\": \"The bank account type.\\n\\nPossible values: **checking** or **savings**. Defaults to **checking**.\",\n      \"enum\": [\n        \"checking\",\n        \"savings\"\n      ],\n      \"type\": \"string\"\n    },\n    \"routingNumber\": {\n      \"description\": \"The 9-digit [routing number](https://en.wikipedia.org/wiki/ABA_routing_transit_number),\
  \ without separators or whitespace.\",\n      \"maxLength\": 9,\n      \"minLength\": 9,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"usLocal\",\n      \"description\": \"**usLocal**\",\n      \"enum\": [\n        \"usLocal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountNumber\",\n    \"routingNumber\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-us-local-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: USLocalAccountIdentification
---
