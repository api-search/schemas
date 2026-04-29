---
description: KYCCheckSummary schema from Adyen API
layout: schema
name: KYCCheckSummary
properties_list:
- description: The code of the check. For possible values, refer to [Verification codes](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/verification-codes).
  name: kycCheckCode
  type: integer
- description: A description of the check.
  name: kycCheckDescription
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-kyc-check-summary-schema.json
slug: accounts-kyc-check-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-kyc-check-summary-schema.json\",\n  \"title\": \"KYCCheckSummary\",\n  \"description\": \"KYCCheckSummary schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kycCheckCode\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The code of the check. For possible values, refer to [Verification codes](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process/verification-codes).\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"kycCheckDescription\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"A description of the check.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-kyc-check-summary-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: KYCCheckSummary
---
