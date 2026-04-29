---
description: PayoutAccountHolderRequest schema from Adyen API
layout: schema
name: PayoutAccountHolderRequest
properties_list:
- description: The code of the account from which the payout is to be made.
  name: accountCode
  type: string
- description: The code of the Account Holder who owns the account from which the payout is to be made. The Account Holder is the party to which the payout will be made.
  name: accountHolderCode
  type: string
- description: An object containing the currency and value of the payout. If the account has multiple currencies, specify the currency to be used. If the `bankAccountUUID` is provided in the request, the currency su
  name: amount
  type: object
- description: The unique ID of the Bank Account held by the Account Holder to which the payout is to be made. If left blank, a bank account is automatically selected.
  name: bankAccountUUID
  type: string
- description: 'A description of the payout. Maximum 200 characters. Allowed: **abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789/?:().,''+ ";**'
  name: description
  type: string
- description: A value that can be supplied at the discretion of the executing user in order to link multiple transactions to one another.
  name: merchantReference
  type: string
- description: The unique ID of the payout method held by the Account Holder to which the payout is to be made. If left blank, a payout instrument is automatically selected.
  name: payoutMethodCode
  type: string
- description: 'Speed with which payouts for this account are processed. Permitted values: `STANDARD`, `SAME_DAY`.'
  name: payoutSpeed
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-payout-account-holder-request-schema.json
slug: funds-payout-account-holder-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-payout-account-holder-request-schema.json\",\n  \"title\": \"PayoutAccountHolderRequest\",\n  \"description\": \"PayoutAccountHolderRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account from which the payout is to be made.\",\n      \"type\": \"string\"\n    },\n    \"accountHolderCode\": {\n      \"description\": \"The code of the Account Holder who owns the account from which the payout is to be made.\\nThe Account Holder is the party to which the payout will be made.\",\n      \"type\": \"string\"\n    },\n    \"amount\": {\n      \"description\": \"An object containing the currency and value of the payout.\\nIf the account has multiple currencies, specify the currency to be used.\\nIf the `bankAccountUUID`\
  \ is provided in the request, the currency supported by the bank is used.\\nIf the `payoutMethodCode` is provided in the request, the specified payout method is selected.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"bankAccountUUID\": {\n      \"description\": \"The unique ID of the Bank Account held by the Account Holder to which the payout is to be made.\\nIf left blank, a bank account is automatically selected.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"A description of the payout. Maximum 200 characters.\\nAllowed: **abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789/?:().,'+ \\\";**\",\n      \"maxLength\": 200,\n      \"type\": \"string\"\n    },\n    \"merchantReference\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"A value that can be supplied at the discretion of the executing user in order to link multiple transactions to one another.\",\n      \"type\": \"string\"\n    },\n  \
  \  \"payoutMethodCode\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The unique ID of the payout method held by the Account Holder to which the payout is to be made.\\nIf left blank, a payout instrument is automatically selected.\",\n      \"type\": \"string\"\n    },\n    \"payoutSpeed\": {\n      \"x-addedInVersion\": \"5\",\n      \"default\": \"STANDARD\",\n      \"description\": \"Speed with which payouts for this account are processed. Permitted values: `STANDARD`, `SAME_DAY`.\",\n      \"enum\": [\n        \"INSTANT\",\n        \"SAME_DAY\",\n        \"STANDARD\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"accountCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-payout-account-holder-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PayoutAccountHolderRequest
---
