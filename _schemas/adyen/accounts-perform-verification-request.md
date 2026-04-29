---
description: PerformVerificationRequest schema from Adyen API
layout: schema
name: PerformVerificationRequest
properties_list:
- description: The code of the account holder to verify.
  name: accountHolderCode
  type: string
- description: 'The state required for the account holder. > Permitted values: `Processing`, `Payout`.'
  name: accountStateType
  type: string
- description: The tier required for the account holder.
  name: tier
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-perform-verification-request-schema.json
slug: accounts-perform-verification-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-perform-verification-request-schema.json\",\n  \"title\": \"PerformVerificationRequest\",\n  \"description\": \"PerformVerificationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder to verify.\",\n      \"type\": \"string\"\n    },\n    \"accountStateType\": {\n      \"description\": \"The state required for the account holder.\\n> Permitted values: `Processing`, `Payout`.\",\n      \"enum\": [\n        \"LimitedPayout\",\n        \"LimitedProcessing\",\n        \"LimitlessPayout\",\n        \"LimitlessProcessing\",\n        \"Payout\",\n        \"Processing\"\n      ],\n      \"type\": \"string\"\n    },\n    \"tier\": {\n      \"description\": \"The tier required for the account holder.\"\
  ,\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"accountStateType\",\n    \"tier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-perform-verification-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PerformVerificationRequest
---
