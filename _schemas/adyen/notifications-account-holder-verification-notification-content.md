---
description: AccountHolderVerificationNotificationContent schema from Adyen API
layout: schema
name: AccountHolderVerificationNotificationContent
properties_list:
- description: The code of the account holder.
  name: accountHolderCode
  type: string
- description: Information on the verification status
  name: kycCheckStatusData
  type: object
- description: The unique ID of the legal arrangement that has been verified.
  name: legalArrangementCode
  type: string
- description: The unique ID of the legal arrangement entity that has been verified.
  name: legalArrangementEntityCode
  type: string
- description: The unique code of the payout method that has been verified.
  name: payoutMethodCode
  type: string
- description: The code of the shareholder that has been verified.
  name: shareholderCode
  type: string
- description: The code of the signatory that has been verified.
  name: signatoryCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-account-holder-verification-notification-content-schema.json
slug: notifications-account-holder-verification-notification-content
source_filename: notifications-account-holder-verification-notification-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-verification-notification-content-schema.json\",\n  \"title\": \"AccountHolderVerificationNotificationContent\",\n  \"description\": \"AccountHolderVerificationNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"kycCheckStatusData\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Information on the verification status\",\n      \"$ref\": \"#/components/schemas/KYCCheckStatusData\"\n    },\n    \"legalArrangementCode\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The unique ID of the legal arrangement that has been verified.\",\n      \"type\": \"string\"\n    },\n    \"legalArrangementEntityCode\"\
  : {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The unique ID of the legal arrangement entity that has been verified.\",\n      \"type\": \"string\"\n    },\n    \"payoutMethodCode\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The unique code of the payout method that has been verified.\",\n      \"type\": \"string\"\n    },\n    \"shareholderCode\": {\n      \"description\": \"The code of the shareholder that has been verified.\",\n      \"type\": \"string\"\n    },\n    \"signatoryCode\": {\n      \"description\": \"The code of the signatory that has been verified.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-verification-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderVerificationNotificationContent
---
