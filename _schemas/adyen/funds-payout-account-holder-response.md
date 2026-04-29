---
description: PayoutAccountHolderResponse schema from Adyen API
layout: schema
name: PayoutAccountHolderResponse
properties_list:
- description: The unique ID of the Bank Account to which the payout was made.
  name: bankAccountUUID
  type: string
- description: Contains field validation errors that would prevent requests from being processed.
  name: invalidFields
  type: array
- description: The value supplied by the executing user when initiating the transfer; may be used to link multiple transactions.
  name: merchantReference
  type: string
- description: 'Speed with which payouts for this account are processed. Permitted values: `STANDARD`, `SAME_DAY`.'
  name: payoutSpeed
  type: string
- description: The reference of a request. Can be used to uniquely identify the request.
  name: pspReference
  type: string
- description: The result code.
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-payout-account-holder-response-schema.json
slug: funds-payout-account-holder-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-payout-account-holder-response-schema.json\",\n  \"title\": \"PayoutAccountHolderResponse\",\n  \"description\": \"PayoutAccountHolderResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankAccountUUID\": {\n      \"description\": \"The unique ID of the Bank Account to which the payout was made.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Contains field validation errors that would prevent requests from being processed.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantReference\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The value supplied by the executing user when initiating\
  \ the transfer; may be used to link multiple transactions.\",\n      \"type\": \"string\"\n    },\n    \"payoutSpeed\": {\n      \"x-addedInVersion\": \"5\",\n      \"default\": \"STANDARD\",\n      \"description\": \"Speed with which payouts for this account are processed. Permitted values: `STANDARD`, `SAME_DAY`.\",\n      \"enum\": [\n        \"INSTANT\",\n        \"SAME_DAY\",\n        \"STANDARD\"\n      ],\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request. Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-payout-account-holder-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PayoutAccountHolderResponse
---
