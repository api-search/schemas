---
description: UtilityRequest schema from Adyen API
layout: schema
name: UtilityRequest
properties_list:
- description: The list of origin domains, for which origin keys are requested.
  name: originDomains
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-utility-request-schema.json
slug: checkout-utility-request
source_filename: checkout-utility-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-utility-request-schema.json\",\n  \"title\": \"UtilityRequest\",\n  \"description\": \"UtilityRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"originDomains\": {\n      \"description\": \"The list of origin domains, for which origin keys are requested.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"originDomains\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-utility-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UtilityRequest
---
