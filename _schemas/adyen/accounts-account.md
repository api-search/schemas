---
description: Account schema from Adyen API
layout: schema
name: Account
properties_list:
- description: The code of the account.
  name: accountCode
  type: string
- description: The bankAccountUUID of the bank account held by the account holder to couple the account with. Scheduled payouts in currencies matching the currency of this bank account will be sent to this bank acco
  name: bankAccountUUID
  type: string
- description: The beneficiary of the account.
  name: beneficiaryAccount
  type: string
- description: The reason that a beneficiary has been set up for this account. This may have been supplied during the setup of a beneficiary at the discretion of the executing user.
  name: beneficiaryMerchantReference
  type: string
- description: A description of the account.
  name: description
  type: string
- description: A set of key and value pairs for general use by the merchant. The keys do not have specific names and may be used for storing miscellaneous data as desired. > Note that during an update of metadata, t
  name: metadata
  type: object
- description: The payout method code held by the account holder to couple the account with. Scheduled card payouts will be sent using this payout method code.
  name: payoutMethodCode
  type: string
- description: The account's payout schedule.
  name: payoutSchedule
  type: object
- description: 'Speed with which payouts for this account are processed. Permitted values: `STANDARD`, `SAME_DAY`.'
  name: payoutSpeed
  type: string
- description: 'The status of the account. Possible values: `Active`, `Inactive`, `Suspended`, `Closed`.'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-account-schema.json
slug: accounts-account
source_filename: accounts-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"Account schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account.\",\n      \"type\": \"string\"\n    },\n    \"bankAccountUUID\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The bankAccountUUID of the bank account held by the account holder to couple the account with. Scheduled payouts in currencies matching the currency of this bank account will be sent to this bank account. Payouts in different currencies will be sent to a matching bank account of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"beneficiaryAccount\": {\n      \"description\": \"The beneficiary of the account.\",\n      \"type\": \"string\"\n\
  \    },\n    \"beneficiaryMerchantReference\": {\n      \"description\": \"The reason that a beneficiary has been set up for this account. This may have been supplied during the setup of a beneficiary at the discretion of the executing user.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"A description of the account.\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"x-addedInVersion\": \"5\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A set of key and value pairs for general use by the merchant.\\nThe keys do not have specific names and may be used for storing miscellaneous data as desired.\\n> Note that during an update of metadata, the omission of existing key-value pairs will result in the deletion of those key-value pairs.\",\n      \"type\": \"object\"\n    },\n    \"payoutMethodCode\": {\n      \"x-addedInVersion\": \"5\",\n  \
  \    \"description\": \"The payout method code held by the account holder to couple the account with. Scheduled card payouts will be sent using this payout method code.\",\n      \"type\": \"string\"\n    },\n    \"payoutSchedule\": {\n      \"description\": \"The account's payout schedule.\",\n      \"$ref\": \"#/components/schemas/PayoutScheduleResponse\"\n    },\n    \"payoutSpeed\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Speed with which payouts for this account are processed. Permitted values: `STANDARD`, `SAME_DAY`.\",\n      \"enum\": [\n        \"INSTANT\",\n        \"SAME_DAY\",\n        \"STANDARD\"\n      ],\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The status of the account. Possible values: `Active`, `Inactive`, `Suspended`, `Closed`.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-account-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Account
---
