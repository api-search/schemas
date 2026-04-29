---
description: KYCCheckResult schema from Adyen API
layout: schema
name: KYCCheckResult
properties_list:
- description: A list of the checks and their statuses.
  name: checks
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-kyc-check-result-schema.json
slug: accounts-kyc-check-result
source_filename: accounts-kyc-check-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-kyc-check-result-schema.json\",\n  \"title\": \"KYCCheckResult\",\n  \"description\": \"KYCCheckResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checks\": {\n      \"description\": \"A list of the checks and their statuses.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KYCCheckStatusData\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-kyc-check-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: KYCCheckResult
---
