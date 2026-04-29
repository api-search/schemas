---
description: UpdateAccountResponse schema from Adyen API
layout: schema
name: UpdateAccountResponse
properties_list:
- description: The code of the account.
  name: accountCode
  type: string
- description: The bankAccountUUID of the bank account held by the account holder to couple the account with. Scheduled payouts in currencies matching the currency of this bank account will be sent to this bank acco
  name: bankAccountUUID
  type: string
- description: The description of the account.
  name: description
  type: string
- description: A list of fields that caused the `/updateAccount` request to fail.
  name: invalidFields
  type: array
- description: A set of key and value pairs containing metadata.
  name: metadata
  type: object
- description: The payout method code held by the account holder to couple the account with. Scheduled card payouts will be sent using this payout method code.
  name: payoutMethodCode
  type: string
- description: The payout schedule of the account.
  name: payoutSchedule
  type: object
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
schema_file: json-schema/notifications-update-account-response-schema.json
slug: notifications-update-account-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-update-account-response-schema.json\",\n  \"title\": \"UpdateAccountResponse\",\n  \"description\": \"UpdateAccountResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account.\",\n      \"type\": \"string\"\n    },\n    \"bankAccountUUID\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The bankAccountUUID of the bank account held by the account holder to couple the account with. Scheduled payouts in currencies matching the currency of this bank account will be sent to this bank account. Payouts in different currencies will be sent to a matching bank account of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\"\
  : \"The description of the account.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"A list of fields that caused the `/updateAccount` request to fail.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"metadata\": {\n      \"x-addedInVersion\": \"5\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A set of key and value pairs containing metadata.\",\n      \"type\": \"object\"\n    },\n    \"payoutMethodCode\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The payout method code held by the account holder to couple the account with. Scheduled card payouts will be sent using this payout method code.\",\n      \"type\": \"string\"\n    },\n    \"payoutSchedule\": {\n      \"description\": \"The payout schedule of the account.\",\n      \"$ref\": \"#/components/schemas/PayoutScheduleResponse\"\
  \n    },\n    \"payoutSpeed\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Speed with which payouts for this account are processed. Permitted values: `STANDARD`, `SAME_DAY`.\",\n      \"enum\": [\n        \"INSTANT\",\n        \"SAME_DAY\",\n        \"STANDARD\"\n      ],\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request. Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-update-account-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdateAccountResponse
---
