---
description: NotificationErrorContainer schema from Adyen API
layout: schema
name: NotificationErrorContainer
properties_list:
- description: The Adyen code that is mapped to the error message.
  name: errorCode
  type: string
- description: A short explanation of the issue.
  name: message
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-notification-error-container-schema.json
slug: notifications-notification-error-container
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-notification-error-container-schema.json\",\n  \"title\": \"NotificationErrorContainer\",\n  \"description\": \"NotificationErrorContainer schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"description\": \"The Adyen code that is mapped to the error message.\",\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"description\": \"A short explanation of the issue.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-notification-error-container-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NotificationErrorContainer
---
