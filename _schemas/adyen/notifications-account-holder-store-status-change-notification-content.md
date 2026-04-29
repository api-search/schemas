---
description: AccountHolderStoreStatusChangeNotificationContent schema from Adyen API
layout: schema
name: AccountHolderStoreStatusChangeNotificationContent
properties_list:
- description: The code of the account holder.
  name: accountHolderCode
  type: string
- description: In case the store status has not been updated, contains fields that did not pass the validation.
  name: invalidFields
  type: array
- description: The new status of the account holder.
  name: newStatus
  type: string
- description: The former status of the account holder.
  name: oldStatus
  type: string
- description: The reason for the status change.
  name: reason
  type: string
- description: Alphanumeric identifier of the store.
  name: store
  type: string
- description: Store store reference.
  name: storeReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-account-holder-store-status-change-notification-content-schema.json
slug: notifications-account-holder-store-status-change-notification-content
source_filename: notifications-account-holder-store-status-change-notification-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-store-status-change-notification-content-schema.json\",\n  \"title\": \"AccountHolderStoreStatusChangeNotificationContent\",\n  \"description\": \"AccountHolderStoreStatusChangeNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The code of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"In case the store status has not been updated, contains fields that did not pass the validation.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"newStatus\": {\n      \"x-addedInVersion\":\
  \ \"5\",\n      \"description\": \"The new status of the account holder.\",\n      \"enum\": [\n        \"Active\",\n        \"Closed\",\n        \"Inactive\",\n        \"InactiveWithModifications\",\n        \"Pending\"\n      ],\n      \"type\": \"string\"\n    },\n    \"oldStatus\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The former status of the account holder.\",\n      \"enum\": [\n        \"Active\",\n        \"Closed\",\n        \"Inactive\",\n        \"InactiveWithModifications\",\n        \"Pending\"\n      ],\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The reason for the status change.\",\n      \"type\": \"string\"\n    },\n    \"store\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Alphanumeric identifier of the store.\",\n      \"type\": \"string\"\n    },\n    \"storeReference\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Store store reference.\"\
  ,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"store\",\n    \"storeReference\",\n    \"oldStatus\",\n    \"newStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-store-status-change-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderStoreStatusChangeNotificationContent
---
