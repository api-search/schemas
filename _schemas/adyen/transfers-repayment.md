---
description: Repayment schema from Adyen API
layout: schema
name: Repayment
properties_list:
- description: The repayment that is deducted daily from incoming net volume, in [basis points](https://www.investopedia.com/terms/b/basispoint.asp).
  name: basisPoints
  type: integer
- description: An object containing the details of the configuration for repayment term.
  name: term
  type: object
- description: An object containing the details of the 30-day repayment threshold.
  name: threshold
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-repayment-schema.json
slug: transfers-repayment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-repayment-schema.json\",\n  \"title\": \"Repayment\",\n  \"description\": \"Repayment schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"basisPoints\": {\n      \"description\": \"The repayment that is deducted daily from incoming net volume, in [basis points](https://www.investopedia.com/terms/b/basispoint.asp).\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"term\": {\n      \"description\": \"An object containing the details of the configuration for repayment term.\",\n      \"$ref\": \"#/components/schemas/RepaymentTerm\"\n    },\n    \"threshold\": {\n      \"description\": \"An object containing the details of the 30-day repayment threshold.\",\n      \"$ref\": \"#/components/schemas/ThresholdRepayment\"\n    }\n  },\n  \"required\": [\n   \
  \ \"basisPoints\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-repayment-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Repayment
---
