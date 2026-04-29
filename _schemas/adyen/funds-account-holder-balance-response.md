---
description: AccountHolderBalanceResponse schema from Adyen API
layout: schema
name: AccountHolderBalanceResponse
properties_list:
- description: A list of each account and their balances.
  name: balancePerAccount
  type: array
- description: Contains field validation errors that would prevent requests from being processed.
  name: invalidFields
  type: array
- description: The reference of a request. Can be used to uniquely identify the request.
  name: pspReference
  type: string
- description: The result code.
  name: resultCode
  type: string
- description: The total balance of the account holder.
  name: totalBalance
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-account-holder-balance-response-schema.json
slug: funds-account-holder-balance-response
source_filename: funds-account-holder-balance-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-account-holder-balance-response-schema.json\",\n  \"title\": \"AccountHolderBalanceResponse\",\n  \"description\": \"AccountHolderBalanceResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balancePerAccount\": {\n      \"description\": \"A list of each account and their balances.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AccountDetailBalance\"\n      },\n      \"type\": \"array\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Contains field validation errors that would prevent requests from being processed.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a\
  \ request. Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    },\n    \"totalBalance\": {\n      \"description\": \"The total balance of the account holder.\",\n      \"$ref\": \"#/components/schemas/DetailBalance\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-account-holder-balance-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderBalanceResponse
---
