---
description: ''
layout: schema
name: CustomerPAN
properties_list:
- description: The card number for which the score needs to be retrieved. A minimum of 16 and a maximum of 19 digits are allowed.
  name: customerPAN
  type: string
- description: A parameter indicating that the user of this API has consent to pull the score for the requested PAN number.
  name: hasConsent
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-consumer-credit-analytics-customer-pan-schema.json
slug: mastercard-consumer-credit-analytics-customer-pan
source_filename: mastercard-consumer-credit-analytics-customer-pan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomerPAN\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerPAN\": {\n      \"type\": \"string\",\n      \"description\": \"The card number for which the score needs to be retrieved. A minimum of 16 and a maximum of 19 digits are allowed.\"\n    },\n    \"hasConsent\": {\n      \"type\": \"boolean\",\n      \"description\": \"A parameter indicating that the user of this API has consent to pull the score for the requested PAN number.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-consumer-credit-analytics-customer-pan-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CustomerPAN
---
