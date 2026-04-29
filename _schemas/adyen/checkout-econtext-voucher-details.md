---
description: EcontextVoucherDetails schema from Adyen API
layout: schema
name: EcontextVoucherDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The shopper's first name.
  name: firstName
  type: string
- description: The shopper's last name.
  name: lastName
  type: string
- description: The shopper's email.
  name: shopperEmail
  type: string
- description: The shopper's contact number. It must have an international number format, for example **+31 20 779 1846**. Formats like **+31 (0)20 779 1846** or **0031 20 779 1846** are not accepted.
  name: telephoneNumber
  type: string
- description: '**econtextvoucher**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-econtext-voucher-details-schema.json
slug: checkout-econtext-voucher-details
source_filename: checkout-econtext-voucher-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-econtext-voucher-details-schema.json\",\n  \"title\": \"EcontextVoucherDetails\",\n  \"description\": \"EcontextVoucherDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"description\": \"The shopper's first name.\",\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"description\": \"The shopper's last name.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper's email.\",\n      \"type\": \"string\"\n    },\n    \"telephoneNumber\": {\n      \"description\": \"The shopper's contact number. It must have an international number\
  \ format, for example **+31 20 779 1846**. Formats like **+31 (0)20 779 1846** or **0031 20 779 1846** are not accepted.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"**econtextvoucher**\",\n      \"enum\": [\n        \"econtext_seveneleven\",\n        \"econtext_stores\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"firstName\",\n    \"lastName\",\n    \"shopperEmail\",\n    \"telephoneNumber\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-econtext-voucher-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: EcontextVoucherDetails
---
