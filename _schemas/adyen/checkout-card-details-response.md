---
description: CardDetailsResponse schema from Adyen API
layout: schema
name: CardDetailsResponse
properties_list:
- description: The list of brands identified for the card.
  name: brands
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-card-details-response-schema.json
slug: checkout-card-details-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-card-details-response-schema.json\",\n  \"title\": \"CardDetailsResponse\",\n  \"description\": \"CardDetailsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brands\": {\n      \"description\": \"The list of brands identified for the card.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CardBrandDetails\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-card-details-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardDetailsResponse
---
