---
description: ThresholdRepayment schema from Adyen API
layout: schema
name: ThresholdRepayment
properties_list:
- description: The amount to be repaid on a 30-day basis.
  name: amount
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-threshold-repayment-schema.json
slug: configuration-threshold-repayment
source_filename: configuration-threshold-repayment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-threshold-repayment-schema.json\",\n  \"title\": \"ThresholdRepayment\",\n  \"description\": \"ThresholdRepayment schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount to be repaid on a 30-day basis.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    }\n  },\n  \"required\": [\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-threshold-repayment-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThresholdRepayment
---
