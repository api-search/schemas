---
description: MbwayDetails schema from Adyen API
layout: schema
name: MbwayDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: ''
  name: shopperEmail
  type: string
- description: ''
  name: telephoneNumber
  type: string
- description: '**mbway**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-mbway-details-schema.json
slug: checkout-mbway-details
source_filename: checkout-mbway-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-mbway-details-schema.json\",\n  \"title\": \"MbwayDetails\",\n  \"description\": \"MbwayDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"\",\n      \"type\": \"string\"\n    },\n    \"telephoneNumber\": {\n      \"description\": \"\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"mbway\",\n      \"description\": \"**mbway**\",\n      \"enum\": [\n        \"mbway\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"telephoneNumber\",\n    \"shopperEmail\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-mbway-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MbwayDetails
---
