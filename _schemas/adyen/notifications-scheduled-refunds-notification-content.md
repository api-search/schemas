---
description: ScheduledRefundsNotificationContent schema from Adyen API
layout: schema
name: ScheduledRefundsNotificationContent
properties_list:
- description: The code of the account.
  name: accountCode
  type: string
- description: The code of the Account Holder.
  name: accountHolderCode
  type: string
- description: Invalid fields list.
  name: invalidFields
  type: array
- description: The most recent payout (after which all transactions were scheduled to be refunded).
  name: lastPayout
  type: object
- description: A list of the refunds that have been scheduled and their results.
  name: refundResults
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-scheduled-refunds-notification-content-schema.json
slug: notifications-scheduled-refunds-notification-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-scheduled-refunds-notification-content-schema.json\",\n  \"title\": \"ScheduledRefundsNotificationContent\",\n  \"description\": \"ScheduledRefundsNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account.\",\n      \"type\": \"string\"\n    },\n    \"accountHolderCode\": {\n      \"description\": \"The code of the Account Holder.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Invalid fields list.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"lastPayout\": {\n      \"description\": \"The most recent payout (after which all transactions\
  \ were scheduled to be refunded).\",\n      \"$ref\": \"#/components/schemas/Transaction\"\n    },\n    \"refundResults\": {\n      \"description\": \"A list of the refunds that have been scheduled and their results.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RefundResult\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-scheduled-refunds-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ScheduledRefundsNotificationContent
---
