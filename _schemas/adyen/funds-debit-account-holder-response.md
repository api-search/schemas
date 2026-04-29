---
description: DebitAccountHolderResponse schema from Adyen API
layout: schema
name: DebitAccountHolderResponse
properties_list:
- description: The code of the account holder.
  name: accountHolderCode
  type: string
- description: The Adyen-generated unique alphanumeric identifier (UUID) of the account holder's bank account.
  name: bankAccountUUID
  type: string
- description: Contains field validation errors that would prevent requests from being processed.
  name: invalidFields
  type: array
- description: List of the `reference` values from the `split` array in the request.
  name: merchantReferences
  type: array
- description: The reference of a request. Can be used to uniquely identify the request.
  name: pspReference
  type: string
- description: The result code.
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-debit-account-holder-response-schema.json
slug: funds-debit-account-holder-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-debit-account-holder-response-schema.json\",\n  \"title\": \"DebitAccountHolderResponse\",\n  \"description\": \"DebitAccountHolderResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"bankAccountUUID\": {\n      \"description\": \"The Adyen-generated unique alphanumeric identifier (UUID) of the account holder's bank account.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Contains field validation errors that would prevent requests from being processed.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n\
  \    },\n    \"merchantReferences\": {\n      \"description\": \"List of the `reference` values from the `split` array in the request.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request. Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-debit-account-holder-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DebitAccountHolderResponse
---
