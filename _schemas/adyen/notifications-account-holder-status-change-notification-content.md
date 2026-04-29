---
description: AccountHolderStatusChangeNotificationContent schema from Adyen API
layout: schema
name: AccountHolderStatusChangeNotificationContent
properties_list:
- description: The code of the account holder.
  name: accountHolderCode
  type: string
- description: in case the account holder has not been updated, contains account holder fields, that did not pass the validation.
  name: invalidFields
  type: array
- description: The new status of the account holder.
  name: newStatus
  type: object
- description: The former status of the account holder.
  name: oldStatus
  type: object
- description: The reason for the status change.
  name: reason
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-account-holder-status-change-notification-content-schema.json
slug: notifications-account-holder-status-change-notification-content
source_filename: notifications-account-holder-status-change-notification-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-status-change-notification-content-schema.json\",\n  \"title\": \"AccountHolderStatusChangeNotificationContent\",\n  \"description\": \"AccountHolderStatusChangeNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"in case the account holder has not been updated, contains account holder fields, that did not pass the validation.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"newStatus\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"\
  The new status of the account holder.\",\n      \"$ref\": \"#/components/schemas/AccountHolderStatus\"\n    },\n    \"oldStatus\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The former status of the account holder.\",\n      \"$ref\": \"#/components/schemas/AccountHolderStatus\"\n    },\n    \"reason\": {\n      \"description\": \"The reason for the status change.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-status-change-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderStatusChangeNotificationContent
---
