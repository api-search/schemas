---
description: NotificationResponse schema from Adyen API
layout: schema
name: NotificationResponse
properties_list:
- description: Set this parameter to **[accepted]** to acknowledge that you received a notification from Adyen.
  name: notificationResponse
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/webhooks-notification-response-schema.json
slug: webhooks-notification-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-notification-response-schema.json\",\n  \"title\": \"NotificationResponse\",\n  \"description\": \"NotificationResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationResponse\": {\n      \"description\": \"Set this parameter to **[accepted]** to acknowledge that you received a notification from Adyen.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-notification-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NotificationResponse
---
