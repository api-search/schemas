---
description: Avs schema from Adyen API
layout: schema
name: Avs
properties_list:
- description: Indicates whether the shopper is allowed to modify the billing address for the current payment request.
  name: addressEditable
  type: boolean
- description: 'Specifies whether the shopper should enter their billing address during checkout. Allowed values: * yes — Perform AVS checks for every card payment. * automatic — Perform AVS checks only when required'
  name: enabled
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-avs-schema.json
slug: checkout-avs
source_filename: checkout-avs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-avs-schema.json\",\n  \"title\": \"Avs\",\n  \"description\": \"Avs schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addressEditable\": {\n      \"description\": \"Indicates whether the shopper is allowed to modify the billing address for the current payment request.\",\n      \"type\": \"boolean\"\n    },\n    \"enabled\": {\n      \"description\": \"Specifies whether the shopper should enter their billing address during checkout.\\n\\nAllowed values:\\n* yes \\u2014 Perform AVS checks for every card payment.\\n* automatic \\u2014 Perform AVS checks only when required to optimize the conversion rate.\\n* no \\u2014 Do not perform AVS checks.\",\n      \"enum\": [\n        \"yes\",\n        \"no\",\n        \"automatic\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-avs-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Avs
---
