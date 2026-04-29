---
description: TestNotificationConfigurationResponse schema from Adyen API
layout: schema
name: TestNotificationConfigurationResponse
properties_list:
- description: Any error messages encountered.
  name: errorMessages
  type: array
- description: 'The event types that were tested. >Permitted values: `ACCOUNT_HOLDER_CREATED`, `ACCOUNT_CREATED`, `ACCOUNT_UPDATED`, `ACCOUNT_HOLDER_UPDATED`, `ACCOUNT_HOLDER_STATUS_CHANGE`, `ACCOUNT_HOLDER_STORE_STA'
  name: eventTypes
  type: array
- description: The notification message and related response messages.
  name: exchangeMessages
  type: array
- description: Contains field validation errors that would prevent requests from being processed.
  name: invalidFields
  type: array
- description: The ID of the notification subscription configuration.
  name: notificationId
  type: integer
- description: A list of messages describing the testing steps.
  name: okMessages
  type: array
- description: The reference of a request. Can be used to uniquely identify the request.
  name: pspReference
  type: string
- description: The result code.
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-configurations-test-notification-configuration-response-schema.json
slug: notification-configurations-test-notification-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-test-notification-configuration-response-schema.json\",\n  \"title\": \"TestNotificationConfigurationResponse\",\n  \"description\": \"TestNotificationConfigurationResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorMessages\": {\n      \"description\": \"Any error messages encountered.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"eventTypes\": {\n      \"description\": \"The event types that were tested.\\n>Permitted values: `ACCOUNT_HOLDER_CREATED`, `ACCOUNT_CREATED`, `ACCOUNT_UPDATED`, `ACCOUNT_HOLDER_UPDATED`, `ACCOUNT_HOLDER_STATUS_CHANGE`, `ACCOUNT_HOLDER_STORE_STATUS_CHANGE` `ACCOUNT_HOLDER_VERIFICATION`, `ACCOUNT_HOLDER_LIMIT_REACHED`, `ACCOUNT_HOLDER_PAYOUT`, `PAYMENT_FAILURE`,\
  \ `SCHEDULED_REFUNDS`, `REPORT_AVAILABLE`, `TRANSFER_FUNDS`, `BENEFICIARY_SETUP`, `COMPENSATE_NEGATIVE_BALANCE`.\",\n      \"items\": {\n        \"enum\": [\n          \"ACCOUNT_CLOSED\",\n          \"ACCOUNT_CREATED\",\n          \"ACCOUNT_FUNDS_BELOW_THRESHOLD\",\n          \"ACCOUNT_HOLDER_CREATED\",\n          \"ACCOUNT_HOLDER_LIMIT_REACHED\",\n          \"ACCOUNT_HOLDER_MIGRATED\",\n          \"ACCOUNT_HOLDER_PAYOUT\",\n          \"ACCOUNT_HOLDER_STATUS_CHANGE\",\n          \"ACCOUNT_HOLDER_STORE_STATUS_CHANGE\",\n          \"ACCOUNT_HOLDER_UPCOMING_DEADLINE\",\n          \"ACCOUNT_HOLDER_UPDATED\",\n          \"ACCOUNT_HOLDER_VERIFICATION\",\n          \"ACCOUNT_UPDATED\",\n          \"BENEFICIARY_SETUP\",\n          \"COMPENSATE_NEGATIVE_BALANCE\",\n          \"DIRECT_DEBIT_INITIATED\",\n          \"FUNDS_MIGRATED\",\n          \"PAYMENT_FAILURE\",\n          \"PENDING_CREDIT\",\n          \"REFUND_FUNDS_TRANSFER\",\n          \"REPORT_AVAILABLE\",\n          \"SCHEDULED_REFUNDS\"\
  ,\n          \"SCORE_SIGNAL_TRIGGERED\",\n          \"TRANSFER_FUNDS\",\n          \"TRANSFER_NOT_PAIDOUT_TRANSFERS\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"exchangeMessages\": {\n      \"description\": \"The notification message and related response messages.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ExchangeMessage\"\n      },\n      \"type\": \"array\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Contains field validation errors that would prevent requests from being processed.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"notificationId\": {\n      \"description\": \"The ID of the notification subscription configuration.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"okMessages\": {\n      \"description\": \"A list of messages describing the\
  \ testing steps.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request. Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"notificationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-test-notification-configuration-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TestNotificationConfigurationResponse
---
