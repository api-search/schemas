---
description: DebitAccountHolderRequest schema from Adyen API
layout: schema
name: DebitAccountHolderRequest
properties_list:
- description: The code of the account holder.
  name: accountHolderCode
  type: string
- description: The amount to be debited from the account holder's bank account.
  name: amount
  type: object
- description: The Adyen-generated unique alphanumeric identifier (UUID) of the account holder's bank account.
  name: bankAccountUUID
  type: string
- description: 'A description of the direct debit. Maximum length: 35 characters. Allowed characters: **a-z**, **A-Z**, **0-9**, and special characters **/?:().,''+ ";**.'
  name: description
  type: string
- description: Your merchant account.
  name: merchantAccount
  type: string
- description: Contains instructions on how to split the funds between the accounts in your platform. The request must have at least one split item.
  name: splits
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-debit-account-holder-request-schema.json
slug: funds-debit-account-holder-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-debit-account-holder-request-schema.json\",\n  \"title\": \"DebitAccountHolderRequest\",\n  \"description\": \"DebitAccountHolderRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"amount\": {\n      \"description\": \"The amount to be debited from the account holder's bank account.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"bankAccountUUID\": {\n      \"description\": \"The Adyen-generated unique alphanumeric identifier (UUID) of the account holder's bank account.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"A description of the direct debit. Maximum length: 35 characters.\\n\\nAllowed\
  \ characters: **a-z**, **A-Z**, **0-9**, and special characters **/?:().,'+ \\\";**.\",\n      \"maxLength\": 35,\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"Your merchant account.\",\n      \"type\": \"string\"\n    },\n    \"splits\": {\n      \"description\": \"Contains instructions on how to split the funds between the accounts in your platform. The request must have at least one split item.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Split\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"bankAccountUUID\",\n    \"amount\",\n    \"splits\",\n    \"merchantAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-debit-account-holder-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DebitAccountHolderRequest
---
