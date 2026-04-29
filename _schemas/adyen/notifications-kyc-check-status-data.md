---
description: KYCCheckStatusData schema from Adyen API
layout: schema
name: KYCCheckStatusData
properties_list:
- description: A list of the fields required for execution of the check.
  name: requiredFields
  type: array
- description: 'The status of the check. Possible values: **AWAITING_DATA** , **DATA_PROVIDED**, **FAILED**, **INVALID_DATA**, **PASSED**, **PENDING**, **RETRY_LIMIT_REACHED**.'
  name: status
  type: string
- description: A summary of the execution of the check.
  name: summary
  type: object
- description: 'The type of check. Possible values: * **BANK_ACCOUNT_VERIFICATION**: Used in v5 and earlier. Replaced by **PAYOUT_METHOD_VERIFICATION** in v6 and later. * **COMPANY_VERIFICATION** * **CARD_VERIFICATIO'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-kyc-check-status-data-schema.json
slug: notifications-kyc-check-status-data
source_filename: notifications-kyc-check-status-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-kyc-check-status-data-schema.json\",\n  \"title\": \"KYCCheckStatusData\",\n  \"description\": \"KYCCheckStatusData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requiredFields\": {\n      \"description\": \"A list of the fields required for execution of the check.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"status\": {\n      \"description\": \"The status of the check.\\n\\nPossible values: **AWAITING_DATA** , **DATA_PROVIDED**, **FAILED**, **INVALID_DATA**, **PASSED**, **PENDING**, **RETRY_LIMIT_REACHED**.\",\n      \"enum\": [\n        \"AWAITING_DATA\",\n        \"DATA_PROVIDED\",\n        \"FAILED\",\n        \"INVALID_DATA\",\n        \"PASSED\",\n        \"PENDING\",\n        \"PENDING_REVIEW\",\n  \
  \      \"RETRY_LIMIT_REACHED\",\n        \"UNCHECKED\"\n      ],\n      \"type\": \"string\"\n    },\n    \"summary\": {\n      \"description\": \"A summary of the execution of the check.\",\n      \"$ref\": \"#/components/schemas/KYCCheckSummary\"\n    },\n    \"type\": {\n      \"description\": \"The type of check.\\n\\nPossible values:\\n\\n * **BANK_ACCOUNT_VERIFICATION**: Used in v5 and earlier. Replaced by **PAYOUT_METHOD_VERIFICATION** in v6 and later.\\n\\n * **COMPANY_VERIFICATION**\\n\\n  * **CARD_VERIFICATION**\\n\\n* **IDENTITY_VERIFICATION**\\n\\n* **LEGAL_ARRANGEMENT_VERIFICATION**\\n\\n* **NONPROFIT_VERIFICATION**\\n\\n * **PASSPORT_VERIFICATION**\\n\\n* **PAYOUT_METHOD_VERIFICATION**: Used in v6 and later.\\n\\n* **PCI_VERIFICATION**\",\n      \"enum\": [\n        \"BANK_ACCOUNT_VERIFICATION\",\n        \"CARD_VERIFICATION\",\n        \"COMPANY_VERIFICATION\",\n        \"IDENTITY_VERIFICATION\",\n        \"LEGAL_ARRANGEMENT_VERIFICATION\",\n        \"NONPROFIT_VERIFICATION\"\
  ,\n        \"PASSPORT_VERIFICATION\",\n        \"PAYOUT_METHOD_VERIFICATION\",\n        \"PCI_VERIFICATION\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-kyc-check-status-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: KYCCheckStatusData
---
