---
description: The error response model used by all of our API endpoints
layout: schema
name: Errors
properties_list:
- description: a list of Error objects
  name: Error
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-errors-schema.json
slug: mastercard-identity-insights-for-transactions-errors
source_filename: mastercard-identity-insights-for-transactions-errors-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Errors\",\n  \"type\": \"object\",\n  \"description\": \"The error response model used by all of our API endpoints\",\n  \"properties\": {\n    \"Error\": {\n      \"type\": \"array\",\n      \"description\": \"a list of Error objects\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-errors-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Errors
---
