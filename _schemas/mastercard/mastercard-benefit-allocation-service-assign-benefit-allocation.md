---
description: ''
layout: schema
name: AssignBenefitAllocation
properties_list:
- description: 16 or 19 digit PAN number that will have a segment assigned to it.
  name: cardNumber
  type: integer
- description: List of segments that will be assigned to the pan number. Only accepts arrays containing one segment.
  name: segments
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-benefit-allocation-service-assign-benefit-allocation-schema.json
slug: mastercard-benefit-allocation-service-assign-benefit-allocation
source_filename: mastercard-benefit-allocation-service-assign-benefit-allocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssignBenefitAllocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"16 or 19 digit PAN number that will have a segment assigned to it.\"\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"List of segments that will be assigned to the pan number. Only accepts arrays containing one segment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-benefit-allocation-service-assign-benefit-allocation-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AssignBenefitAllocation
---
