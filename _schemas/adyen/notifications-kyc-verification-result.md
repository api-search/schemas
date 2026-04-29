---
description: KYCVerificationResult schema from Adyen API
layout: schema
name: KYCVerificationResult
properties_list:
- description: The results of the checks on the account holder.
  name: accountHolder
  type: object
- description: The results of the checks on the legal arrangements.
  name: legalArrangements
  type: array
- description: The results of the checks on the legal arrangement entities.
  name: legalArrangementsEntities
  type: array
- description: The results of the checks on the payout methods.
  name: payoutMethods
  type: array
- description: The results of the checks on the shareholders.
  name: shareholders
  type: array
- description: The results of the checks on the signatories.
  name: signatories
  type: array
- description: The result of the check on the Ultimate Parent Company.
  name: ultimateParentCompany
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-kyc-verification-result-schema.json
slug: notifications-kyc-verification-result
source_filename: notifications-kyc-verification-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-kyc-verification-result-schema.json\",\n  \"title\": \"KYCVerificationResult\",\n  \"description\": \"KYCVerificationResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolder\": {\n      \"description\": \"The results of the checks on the account holder.\",\n      \"$ref\": \"#/components/schemas/KYCCheckResult\"\n    },\n    \"legalArrangements\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The results of the checks on the legal arrangements.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KYCLegalArrangementCheckResult\"\n      },\n      \"type\": \"array\"\n    },\n    \"legalArrangementsEntities\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The results of the checks on the legal arrangement entities.\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KYCLegalArrangementEntityCheckResult\"\n      },\n      \"type\": \"array\"\n    },\n    \"payoutMethods\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The results of the checks on the payout methods.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KYCPayoutMethodCheckResult\"\n      },\n      \"type\": \"array\"\n    },\n    \"shareholders\": {\n      \"description\": \"The results of the checks on the shareholders.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KYCShareholderCheckResult\"\n      },\n      \"type\": \"array\"\n    },\n    \"signatories\": {\n      \"description\": \"The results of the checks on the signatories.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KYCSignatoryCheckResult\"\n      },\n      \"type\": \"array\"\n    },\n    \"ultimateParentCompany\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The result of\
  \ the check on the Ultimate Parent Company.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KYCUltimateParentCompanyCheckResult\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-kyc-verification-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: KYCVerificationResult
---
