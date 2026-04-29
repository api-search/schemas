---
description: AccountHolderCreateNotification schema from Adyen API
layout: schema
name: AccountHolderCreateNotification
properties_list:
- description: The details of the account holder creation.
  name: content
  type: object
- description: Error information of failed request. No value provided here if no error occurred on processing.
  name: error
  type: object
- description: The date and time when an event has been completed.
  name: eventDate
  type: string
- description: The event type of the notification.
  name: eventType
  type: string
- description: The user or process that has triggered the notification.
  name: executingUserKey
  type: string
- description: Indicates whether the notification originated from the live environment or the test environment. If true, the notification originated from the live environment. If false, the notification originated f
  name: live
  type: boolean
- description: The PSP reference of the request from which the notification originates.
  name: pspReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-account-holder-create-notification-schema.json
slug: notifications-account-holder-create-notification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-create-notification-schema.json\",\n  \"title\": \"AccountHolderCreateNotification\",\n  \"description\": \"AccountHolderCreateNotification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"description\": \"The details of the account holder creation.\",\n      \"$ref\": \"#/components/schemas/CreateAccountHolderResponse\"\n    },\n    \"error\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Error information of failed request. No value provided here if no error occurred on processing.\",\n      \"$ref\": \"#/components/schemas/NotificationErrorContainer\"\n    },\n    \"eventDate\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The date and time when an event has been completed.\",\n      \"format\"\
  : \"date-time\",\n      \"type\": \"string\"\n    },\n    \"eventType\": {\n      \"description\": \"The event type of the notification.\",\n      \"type\": \"string\"\n    },\n    \"executingUserKey\": {\n      \"description\": \"The user or process that has triggered the notification.\",\n      \"type\": \"string\"\n    },\n    \"live\": {\n      \"description\": \"Indicates whether the notification originated from the live environment or the test environment. If true, the notification originated from the live environment. If false, the notification originated from the test environment.\",\n      \"type\": \"boolean\"\n    },\n    \"pspReference\": {\n      \"description\": \"The PSP reference of the request from which the notification originates.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"executingUserKey\",\n    \"pspReference\",\n    \"eventType\",\n    \"live\",\n    \"eventDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-create-notification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderCreateNotification
---
