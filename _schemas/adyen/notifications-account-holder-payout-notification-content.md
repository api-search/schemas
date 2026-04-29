---
description: AccountHolderPayoutNotificationContent schema from Adyen API
layout: schema
name: AccountHolderPayoutNotificationContent
properties_list:
- description: The code of the account from which the payout was made.
  name: accountCode
  type: string
- description: The code of the Account Holder to which the payout was made.
  name: accountHolderCode
  type: string
- description: The payout amounts (per currency).
  name: amounts
  type: array
- description: Details of the Bank Account to which the payout was made.
  name: bankAccountDetail
  type: object
- description: A description of the payout.
  name: description
  type: string
- description: The estimated date of arrival.
  name: estimatedArrivalDate
  type: object
- description: Invalid fields list.
  name: invalidFields
  type: array
- description: The merchant reference.
  name: merchantReference
  type: string
- description: The PSP reference of the original payout.
  name: originalPspReference
  type: string
- description: The country code of the bank from which the payout was initiated.
  name: payoutAccountCountry
  type: string
- description: The account number of the bank from which the payout was initiated.
  name: payoutAccountNumber
  type: string
- description: The balance account id to which payment was made
  name: payoutBalanceAccountId
  type: string
- description: The name of the bank the payout from which the payout was initiated.
  name: payoutBankName
  type: string
- description: The branch code of the bank from which the payout was initiated.
  name: payoutBranchCode
  type: string
- description: The unique payout identifier.
  name: payoutReference
  type: integer
- description: 'Speed with which payouts for this account are processed. Permitted values: `STANDARD`, `SAME_DAY`.'
  name: payoutSpeed
  type: string
- description: The payout status.
  name: status
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-account-holder-payout-notification-content-schema.json
slug: notifications-account-holder-payout-notification-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-payout-notification-content-schema.json\",\n  \"title\": \"AccountHolderPayoutNotificationContent\",\n  \"description\": \"AccountHolderPayoutNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account from which the payout was made.\",\n      \"type\": \"string\"\n    },\n    \"accountHolderCode\": {\n      \"description\": \"The code of the Account Holder to which the payout was made.\",\n      \"type\": \"string\"\n    },\n    \"amounts\": {\n      \"description\": \"The payout amounts (per currency).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Amount\"\n      },\n      \"type\": \"array\"\n    },\n    \"bankAccountDetail\": {\n      \"description\": \"Details\
  \ of the Bank Account to which the payout was made.\",\n      \"$ref\": \"#/components/schemas/BankAccountDetail\"\n    },\n    \"description\": {\n      \"description\": \"A description of the payout.\",\n      \"type\": \"string\"\n    },\n    \"estimatedArrivalDate\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The estimated date of arrival.\",\n      \"$ref\": \"#/components/schemas/LocalDate\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Invalid fields list.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantReference\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The merchant reference.\",\n      \"type\": \"string\"\n    },\n    \"originalPspReference\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The PSP reference of the original payout.\",\n      \"type\": \"string\"\n    },\n \
  \   \"payoutAccountCountry\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The country code of the bank from which the payout was initiated.\",\n      \"type\": \"string\"\n    },\n    \"payoutAccountNumber\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The account number of the bank from which the payout was initiated.\",\n      \"type\": \"string\"\n    },\n    \"payoutBalanceAccountId\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The balance account id to which payment was made\",\n      \"type\": \"string\"\n    },\n    \"payoutBankName\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The name of the bank the payout from which the payout was initiated.\",\n      \"type\": \"string\"\n    },\n    \"payoutBranchCode\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The branch code of the bank from which the payout was initiated.\",\n      \"type\": \"string\"\n    },\n    \"payoutReference\"\
  : {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The unique payout identifier.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"payoutSpeed\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Speed with which payouts for this account are processed. Permitted values: `STANDARD`, `SAME_DAY`.\",\n      \"enum\": [\n        \"INSTANT\",\n        \"SAME_DAY\",\n        \"STANDARD\"\n      ],\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The payout status.\",\n      \"$ref\": \"#/components/schemas/OperationStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-payout-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderPayoutNotificationContent
---
