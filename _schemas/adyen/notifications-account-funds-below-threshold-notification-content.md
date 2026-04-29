---
description: AccountFundsBelowThresholdNotificationContent schema from Adyen API
layout: schema
name: AccountFundsBelowThresholdNotificationContent
properties_list:
- description: The code of the account with funds under threshold
  name: accountCode
  type: string
- description: The date of the funds were found to be below threshold.
  name: balanceDate
  type: object
- description: The current funds in the liable account.
  name: currentFunds
  type: object
- description: The configured fund threshold for the liable account
  name: fundThreshold
  type: object
- description: The code of the merchant account.
  name: merchantAccountCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-account-funds-below-threshold-notification-content-schema.json
slug: notifications-account-funds-below-threshold-notification-content
source_filename: notifications-account-funds-below-threshold-notification-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-funds-below-threshold-notification-content-schema.json\",\n  \"title\": \"AccountFundsBelowThresholdNotificationContent\",\n  \"description\": \"AccountFundsBelowThresholdNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account with funds under threshold\",\n      \"type\": \"string\"\n    },\n    \"balanceDate\": {\n      \"description\": \"The date of the funds were found to be below threshold.\",\n      \"$ref\": \"#/components/schemas/LocalDate\"\n    },\n    \"currentFunds\": {\n      \"description\": \"The current funds in the liable account.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"fundThreshold\": {\n      \"description\": \"The configured fund threshold\
  \ for the liable account\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"merchantAccountCode\": {\n      \"description\": \"The code of the merchant account.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccountCode\",\n    \"fundThreshold\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-funds-below-threshold-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountFundsBelowThresholdNotificationContent
---
