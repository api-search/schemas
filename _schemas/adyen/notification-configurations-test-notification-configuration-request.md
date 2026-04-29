---
description: TestNotificationConfigurationRequest schema from Adyen API
layout: schema
name: TestNotificationConfigurationRequest
properties_list:
- description: 'The event types to test. If left blank, then all of the configured event types will be tested. >Permitted values: `ACCOUNT_HOLDER_CREATED`, `ACCOUNT_CREATED`, `ACCOUNT_UPDATED`, `ACCOUNT_HOLDER_UPDATE'
  name: eventTypes
  type: array
- description: The ID of the notification subscription configuration to be tested.
  name: notificationId
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-configurations-test-notification-configuration-request-schema.json
slug: notification-configurations-test-notification-configuration-request
source_filename: notification-configurations-test-notification-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-test-notification-configuration-request-schema.json\",\n  \"title\": \"TestNotificationConfigurationRequest\",\n  \"description\": \"TestNotificationConfigurationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventTypes\": {\n      \"description\": \"The event types to test.  If left blank, then all of the configured event types will be tested.\\n>Permitted values: `ACCOUNT_HOLDER_CREATED`, `ACCOUNT_CREATED`, `ACCOUNT_UPDATED`, `ACCOUNT_HOLDER_UPDATED`, `ACCOUNT_HOLDER_STATUS_CHANGE`, `ACCOUNT_HOLDER_STORE_STATUS_CHANGE` `ACCOUNT_HOLDER_VERIFICATION`, `ACCOUNT_HOLDER_LIMIT_REACHED`, `ACCOUNT_HOLDER_PAYOUT`, `PAYMENT_FAILURE`, `SCHEDULED_REFUNDS`, `REPORT_AVAILABLE`, `TRANSFER_FUNDS`, `BENEFICIARY_SETUP`, `COMPENSATE_NEGATIVE_BALANCE`.\",\n      \"\
  items\": {\n        \"enum\": [\n          \"ACCOUNT_CLOSED\",\n          \"ACCOUNT_CREATED\",\n          \"ACCOUNT_FUNDS_BELOW_THRESHOLD\",\n          \"ACCOUNT_HOLDER_CREATED\",\n          \"ACCOUNT_HOLDER_LIMIT_REACHED\",\n          \"ACCOUNT_HOLDER_MIGRATED\",\n          \"ACCOUNT_HOLDER_PAYOUT\",\n          \"ACCOUNT_HOLDER_STATUS_CHANGE\",\n          \"ACCOUNT_HOLDER_STORE_STATUS_CHANGE\",\n          \"ACCOUNT_HOLDER_UPCOMING_DEADLINE\",\n          \"ACCOUNT_HOLDER_UPDATED\",\n          \"ACCOUNT_HOLDER_VERIFICATION\",\n          \"ACCOUNT_UPDATED\",\n          \"BENEFICIARY_SETUP\",\n          \"COMPENSATE_NEGATIVE_BALANCE\",\n          \"DIRECT_DEBIT_INITIATED\",\n          \"FUNDS_MIGRATED\",\n          \"PAYMENT_FAILURE\",\n          \"PENDING_CREDIT\",\n          \"REFUND_FUNDS_TRANSFER\",\n          \"REPORT_AVAILABLE\",\n          \"SCHEDULED_REFUNDS\",\n          \"SCORE_SIGNAL_TRIGGERED\",\n          \"TRANSFER_FUNDS\",\n          \"TRANSFER_NOT_PAIDOUT_TRANSFERS\"\n   \
  \     ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"notificationId\": {\n      \"description\": \"The ID of the notification subscription configuration to be tested.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"notificationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-test-notification-configuration-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TestNotificationConfigurationRequest
---
