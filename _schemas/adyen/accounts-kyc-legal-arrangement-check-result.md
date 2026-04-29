---
description: KYCLegalArrangementCheckResult schema from Adyen API
layout: schema
name: KYCLegalArrangementCheckResult
properties_list:
- description: A list of the checks and their statuses.
  name: checks
  type: array
- description: The unique ID of the legal arrangement to which the check applies.
  name: legalArrangementCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-kyc-legal-arrangement-check-result-schema.json
slug: accounts-kyc-legal-arrangement-check-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-kyc-legal-arrangement-check-result-schema.json\",\n  \"title\": \"KYCLegalArrangementCheckResult\",\n  \"description\": \"KYCLegalArrangementCheckResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checks\": {\n      \"description\": \"A list of the checks and their statuses.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KYCCheckStatusData\"\n      },\n      \"type\": \"array\"\n    },\n    \"legalArrangementCode\": {\n      \"description\": \"The unique ID of the legal arrangement to which the check applies.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-kyc-legal-arrangement-check-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: KYCLegalArrangementCheckResult
---
