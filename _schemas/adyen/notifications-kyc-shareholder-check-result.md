---
description: KYCShareholderCheckResult schema from Adyen API
layout: schema
name: KYCShareholderCheckResult
properties_list:
- description: A list of the checks and their statuses.
  name: checks
  type: array
- description: The unique ID of the legal arrangement to which the shareholder belongs, if applicable.
  name: legalArrangementCode
  type: string
- description: The unique ID of the legal arrangement entity to which the shareholder belongs, if applicable.
  name: legalArrangementEntityCode
  type: string
- description: The code of the shareholder to which the check applies.
  name: shareholderCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-kyc-shareholder-check-result-schema.json
slug: notifications-kyc-shareholder-check-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-kyc-shareholder-check-result-schema.json\",\n  \"title\": \"KYCShareholderCheckResult\",\n  \"description\": \"KYCShareholderCheckResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checks\": {\n      \"description\": \"A list of the checks and their statuses.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KYCCheckStatusData\"\n      },\n      \"type\": \"array\"\n    },\n    \"legalArrangementCode\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The unique ID of the legal arrangement to which the shareholder belongs, if applicable.\",\n      \"type\": \"string\"\n    },\n    \"legalArrangementEntityCode\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The unique ID of the legal arrangement entity to which the shareholder\
  \ belongs, if applicable.\",\n      \"type\": \"string\"\n    },\n    \"shareholderCode\": {\n      \"description\": \"The code of the shareholder to which the check applies.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-kyc-shareholder-check-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: KYCShareholderCheckResult
---
