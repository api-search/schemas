---
description: GetTerminalsUnderAccountResponse schema from Adyen API
layout: schema
name: GetTerminalsUnderAccountResponse
properties_list:
- description: Your company account.
  name: companyAccount
  type: string
- description: Array that returns a list of all terminals that are in the inventory of the company account.
  name: inventoryTerminals
  type: array
- description: Array that returns a list of all merchant accounts belonging to the company account.
  name: merchantAccounts
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/pos-terminal-get-terminals-under-account-response-schema.json
slug: pos-terminal-get-terminals-under-account-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-get-terminals-under-account-response-schema.json\",\n  \"title\": \"GetTerminalsUnderAccountResponse\",\n  \"description\": \"GetTerminalsUnderAccountResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyAccount\": {\n      \"description\": \"Your company account.\",\n      \"type\": \"string\"\n    },\n    \"inventoryTerminals\": {\n      \"description\": \"Array that returns a list of all terminals that are in the inventory of the company account.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantAccounts\": {\n      \"description\": \"Array that returns a list of all merchant accounts belonging to the company account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MerchantAccount\"\
  \n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"companyAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-get-terminals-under-account-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetTerminalsUnderAccountResponse
---
