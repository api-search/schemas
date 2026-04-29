---
description: CancelOrderResponse schema from Adyen API
layout: schema
name: CancelOrderResponse
properties_list:
- description: A unique reference of the cancellation request.
  name: pspReference
  type: string
- description: 'The result of the cancellation request. Possible values: * **Received** – Indicates the cancellation has successfully been received by Adyen, and will be processed.'
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-cancel-order-response-schema.json
slug: checkout-cancel-order-response
source_filename: checkout-cancel-order-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-cancel-order-response-schema.json\",\n  \"title\": \"CancelOrderResponse\",\n  \"description\": \"CancelOrderResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pspReference\": {\n      \"description\": \"A unique reference of the cancellation request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result of the cancellation request.\\n\\nPossible values:\\n\\n* **Received** \\u2013 Indicates the cancellation has successfully been received by Adyen, and will be processed.\",\n      \"enum\": [\n        \"Received\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"pspReference\",\n    \"resultCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-cancel-order-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CancelOrderResponse
---
