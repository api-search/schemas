---
description: ''
layout: schema
name: ReplaceBenefitAllocation
properties_list:
- description: 16 or 19 digit PAN number that will have its segment replaced.
  name: cardNumber
  type: integer
- description: Unique identifier representing a group of benefit bundles that will be expired and replaced.
  name: oldSegmentCode
  type: string
- description: Unique identifier representing the new group of benefit bundles that will be assigned.
  name: newSegmentCode
  type: string
- description: Date at which the new segment will go in effect. Date should be in YYYY-MM-DD format.
  name: effectiveDate
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-benefit-allocation-service-replace-benefit-allocation-schema.json
slug: mastercard-benefit-allocation-service-replace-benefit-allocation
source_filename: mastercard-benefit-allocation-service-replace-benefit-allocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplaceBenefitAllocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"16 or 19 digit PAN number that will have its segment replaced.\"\n    },\n    \"oldSegmentCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier representing a group of benefit bundles that will be expired and replaced.\"\n    },\n    \"newSegmentCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier representing the new group of benefit bundles that will be assigned.\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date at which the new segment will go in effect. Date should be in YYYY-MM-DD format.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-benefit-allocation-service-replace-benefit-allocation-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ReplaceBenefitAllocation
---
