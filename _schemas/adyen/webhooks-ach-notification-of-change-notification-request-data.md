---
description: AchNotificationOfChangeNotificationRequestData schema from Adyen API
layout: schema
name: AchNotificationOfChangeNotificationRequestData
properties_list:
- description: The Notification of Change information.
  name: notificationOfChange
  type: object
- description: PSP Reference.
  name: pspReference
  type: string
- description: Shopper reference.
  name: shopperReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/webhooks-ach-notification-of-change-notification-request-data-schema.json
slug: webhooks-ach-notification-of-change-notification-request-data
source_filename: webhooks-ach-notification-of-change-notification-request-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-ach-notification-of-change-notification-request-data-schema.json\",\n  \"title\": \"AchNotificationOfChangeNotificationRequestData\",\n  \"description\": \"AchNotificationOfChangeNotificationRequestData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationOfChange\": {\n      \"description\": \"The Notification of Change information.\",\n      \"$ref\": \"#/components/schemas/AchNotificationOfChangeNotificationRequestDataNoc\"\n    },\n    \"pspReference\": {\n      \"description\": \"PSP Reference.\",\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"Shopper reference.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"pspReference\",\n    \"shopperReference\",\n    \"notificationOfChange\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-ach-notification-of-change-notification-request-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AchNotificationOfChangeNotificationRequestData
---
