---
description: ''
layout: schema
name: Errors
properties_list:
- description: Errors array wrapped in an error object
  name: Error
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-errors-schema.json
slug: mastercard-card-issuance-errors
source_filename: mastercard-card-issuance-errors-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Errors\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Error\": {\n      \"type\": \"array\",\n      \"description\": \"Errors array wrapped in an error object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-errors-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Errors
---
