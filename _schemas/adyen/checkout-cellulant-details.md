---
description: CellulantDetails schema from Adyen API
layout: schema
name: CellulantDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The Cellulant issuer.
  name: issuer
  type: string
- description: '**Cellulant**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-cellulant-details-schema.json
slug: checkout-cellulant-details
source_filename: checkout-cellulant-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-cellulant-details-schema.json\",\n  \"title\": \"CellulantDetails\",\n  \"description\": \"CellulantDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"issuer\": {\n      \"description\": \"The Cellulant issuer.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"cellulant\",\n      \"description\": \"**Cellulant**\",\n      \"enum\": [\n        \"cellulant\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-cellulant-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CellulantDetails
---
