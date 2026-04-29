---
description: ''
layout: schema
name: Bundles
properties_list:
- description: List of eligible benefit bundles after a segment has been assigned to a card number.
  name: bundles
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-benefit-allocation-service-bundles-schema.json
slug: mastercard-benefit-allocation-service-bundles
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Bundles\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bundles\": {\n      \"type\": \"array\",\n      \"description\": \"List of eligible benefit bundles after a segment has been assigned to a card number.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-benefit-allocation-service-bundles-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Bundles
---
