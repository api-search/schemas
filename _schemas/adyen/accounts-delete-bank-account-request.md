---
description: DeleteBankAccountRequest schema from Adyen API
layout: schema
name: DeleteBankAccountRequest
properties_list:
- description: The code of the Account Holder from which to delete the Bank Account(s).
  name: accountHolderCode
  type: string
- description: The code(s) of the Bank Accounts to be deleted.
  name: bankAccountUUIDs
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-delete-bank-account-request-schema.json
slug: accounts-delete-bank-account-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-delete-bank-account-request-schema.json\",\n  \"title\": \"DeleteBankAccountRequest\",\n  \"description\": \"DeleteBankAccountRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the Account Holder from which to delete the Bank Account(s).\",\n      \"type\": \"string\"\n    },\n    \"bankAccountUUIDs\": {\n      \"description\": \"The code(s) of the Bank Accounts to be deleted.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"bankAccountUUIDs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-delete-bank-account-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DeleteBankAccountRequest
---
