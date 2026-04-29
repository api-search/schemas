---
description: RiskData schema from Adyen API
layout: schema
name: RiskData
properties_list:
- description: Contains client-side data, like the device fingerprint, cookies, and specific browser settings.
  name: clientData
  type: string
- description: Any custom fields used as part of the input to configured risk rules.
  name: customFields
  type: object
- description: An integer value that is added to the normal fraud score. The value can be either positive or negative.
  name: fraudOffset
  type: integer
- description: The risk profile to assign to this payment. When left empty, the merchant-level account's default risk profile will be applied.
  name: profileReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-risk-data-schema.json
slug: checkout-risk-data
source_filename: checkout-risk-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-risk-data-schema.json\",\n  \"title\": \"RiskData\",\n  \"description\": \"RiskData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientData\": {\n      \"description\": \"Contains client-side data, like the device fingerprint, cookies, and specific browser settings.\",\n      \"type\": \"string\"\n    },\n    \"customFields\": {\n      \"x-addedInVersion\": \"65\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Any custom fields used as part of the input to configured risk rules.\",\n      \"type\": \"object\"\n    },\n    \"fraudOffset\": {\n      \"x-addedInVersion\": \"65\",\n      \"description\": \"An integer value that is added to the normal fraud score. The value can be either positive or negative.\",\n      \"\
  format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"profileReference\": {\n      \"x-addedInVersion\": \"65\",\n      \"description\": \"The risk profile to assign to this payment. When left empty, the merchant-level account's default risk profile will be applied.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-risk-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RiskData
---
