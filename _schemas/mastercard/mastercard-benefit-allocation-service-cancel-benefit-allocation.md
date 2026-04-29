---
description: ''
layout: schema
name: CancelBenefitAllocation
properties_list:
- description: 16 or 19 digit PAN number that will have it's segment expired/cancelled.
  name: cardNumber
  type: integer
- description: List of segments assigned to the card number that will be cancelled. Only accepts arrays containing one segment.
  name: segments
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-benefit-allocation-service-cancel-benefit-allocation-schema.json
slug: mastercard-benefit-allocation-service-cancel-benefit-allocation
source_filename: mastercard-benefit-allocation-service-cancel-benefit-allocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CancelBenefitAllocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"16 or 19 digit PAN number that will have it's segment expired/cancelled.\"\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"List of segments assigned to the card number that will be cancelled. Only accepts arrays containing one segment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-benefit-allocation-service-cancel-benefit-allocation-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CancelBenefitAllocation
---
