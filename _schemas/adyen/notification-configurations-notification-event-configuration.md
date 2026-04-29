---
description: NotificationEventConfiguration schema from Adyen API
layout: schema
name: NotificationEventConfiguration
properties_list:
- description: 'The type of event. Possible values: **ACCOUNT_CLOSED**, **ACCOUNT_CREATED**, **ACCOUNT_FUNDS_BELOW_THRESHOLD**, **ACCOUNT_HOLDER_CREATED**, **ACCOUNT_HOLDER_LIMIT_REACHED**, **ACCOUNT_HOLDER_PAYOUT**,'
  name: eventType
  type: string
- description: 'Indicates whether the specified `eventType` is sent to your webhook endpoint. Possible values: * **INCLUDE**: Send the specified `eventType`. * **EXCLUDE**: Send all event types except the specified `'
  name: includeMode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-configurations-notification-event-configuration-schema.json
slug: notification-configurations-notification-event-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-notification-event-configuration-schema.json\",\n  \"title\": \"NotificationEventConfiguration\",\n  \"description\": \"NotificationEventConfiguration schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventType\": {\n      \"description\": \"The type of event.\\n\\nPossible values: **ACCOUNT_CLOSED**, **ACCOUNT_CREATED**, **ACCOUNT_FUNDS_BELOW_THRESHOLD**, **ACCOUNT_HOLDER_CREATED**, **ACCOUNT_HOLDER_LIMIT_REACHED**, **ACCOUNT_HOLDER_PAYOUT**, **ACCOUNT_HOLDER_STATUS_CHANGE**, **ACCOUNT_HOLDER_STORE_STATUS_CHANGE**, **ACCOUNT_HOLDER_UPCOMING_DEADLINE**, **ACCOUNT_HOLDER_UPDATED**, **ACCOUNT_HOLDER_VERIFICATION**, **ACCOUNT_UPDATED**, **BENEFICIARY_SETUP**, **COMPENSATE_NEGATIVE_BALANCE**, **DIRECT_DEBIT_INITIATED**, **PAYMENT_FAILURE**, **REFUND_FUNDS_TRANSFER**,\
  \ **REPORT_AVAILABLE**, **SCHEDULED_REFUNDS**, **TRANSFER_FUNDS**.\",\n      \"enum\": [\n        \"ACCOUNT_CLOSED\",\n        \"ACCOUNT_CREATED\",\n        \"ACCOUNT_FUNDS_BELOW_THRESHOLD\",\n        \"ACCOUNT_HOLDER_CREATED\",\n        \"ACCOUNT_HOLDER_LIMIT_REACHED\",\n        \"ACCOUNT_HOLDER_MIGRATED\",\n        \"ACCOUNT_HOLDER_PAYOUT\",\n        \"ACCOUNT_HOLDER_STATUS_CHANGE\",\n        \"ACCOUNT_HOLDER_STORE_STATUS_CHANGE\",\n        \"ACCOUNT_HOLDER_UPCOMING_DEADLINE\",\n        \"ACCOUNT_HOLDER_UPDATED\",\n        \"ACCOUNT_HOLDER_VERIFICATION\",\n        \"ACCOUNT_UPDATED\",\n        \"BENEFICIARY_SETUP\",\n        \"COMPENSATE_NEGATIVE_BALANCE\",\n        \"DIRECT_DEBIT_INITIATED\",\n        \"FUNDS_MIGRATED\",\n        \"PAYMENT_FAILURE\",\n        \"PENDING_CREDIT\",\n        \"REFUND_FUNDS_TRANSFER\",\n        \"REPORT_AVAILABLE\",\n        \"SCHEDULED_REFUNDS\",\n        \"SCORE_SIGNAL_TRIGGERED\",\n        \"TRANSFER_FUNDS\",\n        \"TRANSFER_NOT_PAIDOUT_TRANSFERS\"\
  \n      ],\n      \"type\": \"string\"\n    },\n    \"includeMode\": {\n      \"description\": \"Indicates whether the specified `eventType` is sent to your webhook endpoint.\\nPossible values:\\n* **INCLUDE**: Send the specified `eventType`.\\n* **EXCLUDE**: Send all event types except the specified `eventType` and other event types with the `includeMode` set to **EXCLUDE**.\",\n      \"enum\": [\n        \"EXCLUDE\",\n        \"INCLUDE\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"eventType\",\n    \"includeMode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-notification-event-configuration-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NotificationEventConfiguration
---
