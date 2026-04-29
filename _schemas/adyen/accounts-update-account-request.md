---
description: UpdateAccountRequest schema from Adyen API
layout: schema
name: UpdateAccountRequest
properties_list:
- description: The code of the account to update.
  name: accountCode
  type: string
- description: The bankAccountUUID of the bank account held by the account holder to couple the account with. Scheduled payouts in currencies matching the currency of this bank account will be sent to this bank acco
  name: bankAccountUUID
  type: string
- description: A description of the account, maximum 256 characters.You can use alphanumeric characters (A-Z, a-z, 0-9), white spaces, and underscores `_`.
  name: description
  type: string
- description: A set of key and value pairs for general use by the merchant. The keys do not have specific names and may be used for storing miscellaneous data as desired. > Note that during an update of metadata, t
  name: metadata
  type: object
- description: The payout method code held by the account holder to couple the account with. Scheduled card payouts will be sent using this payout method code.
  name: payoutMethodCode
  type: string
- description: The details of the payout schedule, to which the account should be updated.
  name: payoutSchedule
  type: object
- description: 'Speed with which payouts for this account are processed. Permitted values: `STANDARD`, `SAME_DAY`.'
  name: payoutSpeed
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-update-account-request-schema.json
slug: accounts-update-account-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-update-account-request-schema.json\",\n  \"title\": \"UpdateAccountRequest\",\n  \"description\": \"UpdateAccountRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account to update.\",\n      \"type\": \"string\"\n    },\n    \"bankAccountUUID\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The bankAccountUUID of the bank account held by the account holder to couple the account with. Scheduled payouts in currencies matching the currency of this bank account will be sent to this bank account. Payouts in different currencies will be sent to a matching bank account of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"4\",\n      \"\
  description\": \"A description of the account, maximum 256 characters.You can use alphanumeric characters (A-Z, a-z, 0-9), white spaces, and underscores `_`.\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"x-addedInVersion\": \"5\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A set of key and value pairs for general use by the merchant.\\nThe keys do not have specific names and may be used for storing miscellaneous data as desired.\\n> Note that during an update of metadata, the omission of existing key-value pairs will result in the deletion of those key-value pairs.\",\n      \"type\": \"object\"\n    },\n    \"payoutMethodCode\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The payout method code held by the account holder to couple the account with. Scheduled card payouts will be sent using this payout method code.\",\n      \"type\": \"string\"\n    },\n    \"payoutSchedule\": {\n    \
  \  \"description\": \"The details of the payout schedule, to which the account should be updated.\",\n      \"$ref\": \"#/components/schemas/UpdatePayoutScheduleRequest\"\n    },\n    \"payoutSpeed\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Speed with which payouts for this account are processed. Permitted values: `STANDARD`, `SAME_DAY`.\",\n      \"enum\": [\n        \"INSTANT\",\n        \"SAME_DAY\",\n        \"STANDARD\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-update-account-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdateAccountRequest
---
