---
description: MasterpassDetails schema from Adyen API
layout: schema
name: MasterpassDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The funding source that should be used when multiple sources are available. For Brazilian combo cards, by default the funding source is credit. To use debit, set this value to **debit**.
  name: fundingSource
  type: string
- description: The Masterpass transaction ID.
  name: masterpassTransactionId
  type: string
- description: '**masterpass**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-masterpass-details-schema.json
slug: checkout-masterpass-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-masterpass-details-schema.json\",\n  \"title\": \"MasterpassDetails\",\n  \"description\": \"MasterpassDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"fundingSource\": {\n      \"description\": \"The funding source that should be used when multiple sources are available. For Brazilian combo cards, by default the funding source is credit. To use debit, set this value to **debit**.\",\n      \"enum\": [\n        \"credit\",\n        \"debit\"\n      ],\n      \"type\": \"string\"\n    },\n    \"masterpassTransactionId\": {\n      \"description\": \"The Masterpass transaction ID.\",\n      \"type\": \"string\"\
  \n    },\n    \"type\": {\n      \"default\": \"masterpass\",\n      \"description\": \"**masterpass**\",\n      \"enum\": [\n        \"masterpass\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"masterpassTransactionId\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-masterpass-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MasterpassDetails
---
