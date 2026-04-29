---
description: ''
layout: schema
name: BundleDetails
properties_list:
- description: Unique identifier of a benefit bundle that represents a group of benefit instances available.
  name: code
  type: string
- description: Effective date associated to the benefits in the benefit bundle. Date will be in YYYY-MM-DD format.
  name: effectiveDate
  type: string
- description: Expiry date associated to the benefits in the benefit bundle. Date will be in YYYY-MM-DD format.
  name: expiryDate
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-benefit-allocation-service-bundle-details-schema.json
slug: mastercard-benefit-allocation-service-bundle-details
source_filename: mastercard-benefit-allocation-service-bundle-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BundleDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of a benefit bundle that represents a group of benefit instances available.\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"Effective date associated to the benefits in the benefit bundle. Date will be in YYYY-MM-DD format.\"\n    },\n    \"expiryDate\": {\n      \"type\": \"string\",\n      \"description\": \"Expiry date associated to the benefits in the benefit bundle. Date will be in YYYY-MM-DD format.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-benefit-allocation-service-bundle-details-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: BundleDetails
---
