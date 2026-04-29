---
description: ''
layout: schema
name: SegmentToCancel
properties_list:
- description: Identifier that represents a group of benefit bundles to be cancelled.
  name: code
  type: string
- description: Date at which the benefit bundles associated to the segment code will be cancelled. Date should be in YYYY-MM-DD format.
  name: expiryDate
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-benefit-allocation-service-segment-to-cancel-schema.json
slug: mastercard-benefit-allocation-service-segment-to-cancel
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SegmentToCancel\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that represents a group of benefit bundles to be cancelled.\"\n    },\n    \"expiryDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date at which the benefit bundles associated to the segment code will be cancelled. Date should be in YYYY-MM-DD format.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-benefit-allocation-service-segment-to-cancel-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: SegmentToCancel
---
