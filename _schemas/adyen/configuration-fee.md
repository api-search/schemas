---
description: Fee schema from Adyen API
layout: schema
name: Fee
properties_list:
- description: An object containing the fee amount.
  name: amount
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-fee-schema.json
slug: configuration-fee
source_filename: configuration-fee-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-fee-schema.json\",\n  \"title\": \"Fee\",\n  \"description\": \"Fee schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"An object containing the fee amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    }\n  },\n  \"required\": [\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-fee-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Fee
---
