---
description: ''
layout: schema
name: Segment
properties_list:
- description: Unique identifier representing a group of benefit bundles to be assigned.
  name: code
  type: string
- description: Date at which the benefit bundles associated to the segment code will be active and available for use. Date should be in YYYY-MM-DD format.
  name: effectiveDate
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-benefit-allocation-service-segment-schema.json
slug: mastercard-benefit-allocation-service-segment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Segment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier representing a group of benefit bundles to be assigned.\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date at which the benefit bundles associated to the segment code will be active and available for use. Date should be in YYYY-MM-DD format.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-benefit-allocation-service-segment-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Segment
---
