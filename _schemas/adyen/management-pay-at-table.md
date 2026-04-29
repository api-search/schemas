---
description: PayAtTable schema from Adyen API
layout: schema
name: PayAtTable
properties_list:
- description: 'Allowed authentication methods: Magswipe, Manual Entry.'
  name: authenticationMethod
  type: string
- description: Enable Pay at table.
  name: enablePayAtTable
  type: boolean
- description: 'Sets the allowed payment instrument for Pay at table transactions. Can be: **cash** or **card**. If not set, the terminal presents both options.'
  name: paymentInstrument
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-pay-at-table-schema.json
slug: management-pay-at-table
source_filename: management-pay-at-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-pay-at-table-schema.json\",\n  \"title\": \"PayAtTable\",\n  \"description\": \"PayAtTable schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authenticationMethod\": {\n      \"description\": \"Allowed authentication methods: Magswipe, Manual Entry.\",\n      \"enum\": [\n        \"MAGSWIPE\",\n        \"MKE\"\n      ],\n      \"type\": \"string\"\n    },\n    \"enablePayAtTable\": {\n      \"description\": \"Enable Pay at table.\",\n      \"type\": \"boolean\"\n    },\n    \"paymentInstrument\": {\n      \"description\": \"Sets the allowed payment instrument for Pay at table transactions.  Can be: **cash** or **card**. If not set, the terminal presents both options.\",\n      \"enum\": [\n        \"Cash\",\n        \"Card\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-pay-at-table-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PayAtTable
---
