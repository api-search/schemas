---
description: ''
layout: schema
name: ErrorData
properties_list:
- description: A short description of the ErrorCode field.
  name: reasonCode
  type: string
- description: A detailed description of the Error.
  name: errorMessage
  type: string
- description: Name of the model used for scoring against customerPANs.
  name: modelName
  type: string
- description: A score type for which score is not retrieved.
  name: scoreType
  type: string
- description: A product type for which score is not retrieved.
  name: productType
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-consumer-credit-analytics-error-data-schema.json
slug: mastercard-consumer-credit-analytics-error-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorData\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of the ErrorCode field.\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the Error.\"\n    },\n    \"modelName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the model used for scoring against customerPANs.\"\n    },\n    \"scoreType\": {\n      \"type\": \"string\",\n      \"description\": \"A score type for which score is not retrieved.\"\n    },\n    \"productType\": {\n      \"type\": \"string\",\n      \"description\": \"A product type for which score is not retrieved.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-consumer-credit-analytics-error-data-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ErrorData
---
