---
description: NotificationModificationData schema from Adyen API
layout: schema
name: NotificationModificationData
properties_list:
- description: The amount of the modification converted to the balance account's currency, in case the original transaction currency is different. For example, if a part of an authorised amount was cancelled, the va
  name: amount
  type: object
- description: 'The type of modification. Possible values: **Authorised**, **Cancelled**, **Captured**, **Error**, **Expired**, **OutgoingTransfer**, **PendingIncomingTransfer**, **PendingRefund**, **IncomingTransfer'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-notification-modification-data-schema.json
slug: notification-webhooks-notification-modification-data
source_filename: notification-webhooks-notification-modification-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-notification-modification-data-schema.json\",\n  \"title\": \"NotificationModificationData\",\n  \"description\": \"NotificationModificationData schema from Adyen API\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount of the modification converted to the balance account's currency, in case the original transaction currency is different. For example, if a part of an authorised amount was cancelled, the value shows the amount that was cancelled.\\n\\n * A _positive_ value means the amount is added to the balance account.\\n\\n * A _negative_ value means the amount is deducted from the balance account. \",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"type\": {\n      \"description\": \"The type of modification.\\n\\nPossible values: **Authorised**,\
  \ **Cancelled**, **Captured**, **Error**, **Expired**, **OutgoingTransfer**, **PendingIncomingTransfer**, **PendingRefund**, **IncomingTransfer**, **Refunded**, **Refused**.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-notification-modification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NotificationModificationData
---
