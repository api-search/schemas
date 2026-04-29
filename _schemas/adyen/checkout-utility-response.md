---
description: UtilityResponse schema from Adyen API
layout: schema
name: UtilityResponse
properties_list:
- description: The list of origin keys for all requested domains. For each list item, the key is the domain and the value is the origin key.
  name: originKeys
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-utility-response-schema.json
slug: checkout-utility-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-utility-response-schema.json\",\n  \"title\": \"UtilityResponse\",\n  \"description\": \"UtilityResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"originKeys\": {\n      \"x-addedInVersion\": \"1\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The list of origin keys for all requested domains. For each list item, the key is the domain and the value is the origin key.\",\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-utility-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UtilityResponse
---
