---
description: TokenDetails schema from Adyen API
layout: schema
name: TokenDetails
properties_list:
- description: ''
  name: tokenData
  type: object
- description: ''
  name: tokenDataType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-token-details-schema.json
slug: recurring-token-details
source_filename: recurring-token-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-token-details-schema.json\",\n  \"title\": \"TokenDetails\",\n  \"description\": \"TokenDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tokenData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"object\"\n    },\n    \"tokenDataType\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-token-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TokenDetails
---
