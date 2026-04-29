---
description: CardBrandDetails schema from Adyen API
layout: schema
name: CardBrandDetails
properties_list:
- description: Indicates if you support the card brand.
  name: supported
  type: boolean
- description: The name of the card brand.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-card-brand-details-schema.json
slug: checkout-card-brand-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-card-brand-details-schema.json\",\n  \"title\": \"CardBrandDetails\",\n  \"description\": \"CardBrandDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"supported\": {\n      \"description\": \"Indicates if you support the card brand.\",\n      \"type\": \"boolean\"\n    },\n    \"type\": {\n      \"description\": \"The name of the card brand.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-card-brand-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardBrandDetails
---
