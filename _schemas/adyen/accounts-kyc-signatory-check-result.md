---
description: KYCSignatoryCheckResult schema from Adyen API
layout: schema
name: KYCSignatoryCheckResult
properties_list:
- description: A list of the checks and their statuses.
  name: checks
  type: array
- description: The code of the signatory to which the check applies.
  name: signatoryCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-kyc-signatory-check-result-schema.json
slug: accounts-kyc-signatory-check-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-kyc-signatory-check-result-schema.json\",\n  \"title\": \"KYCSignatoryCheckResult\",\n  \"description\": \"KYCSignatoryCheckResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checks\": {\n      \"description\": \"A list of the checks and their statuses.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KYCCheckStatusData\"\n      },\n      \"type\": \"array\"\n    },\n    \"signatoryCode\": {\n      \"description\": \"The code of the signatory to which the check applies.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-kyc-signatory-check-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: KYCSignatoryCheckResult
---
