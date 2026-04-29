---
description: AccountNotificationResponse schema from Adyen API
layout: schema
name: AccountNotificationResponse
properties_list:
- description: Respond with **HTTP 200 OK** and `[accepted]` in the response body to [accept the webhook](https://docs.adyen.com/development-resources/webhooks#accept-notifications).
  name: notificationResponse
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-webhooks-account-notification-response-schema.json
slug: management-webhooks-account-notification-response
source_filename: management-webhooks-account-notification-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-account-notification-response-schema.json\",\n  \"title\": \"AccountNotificationResponse\",\n  \"description\": \"AccountNotificationResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationResponse\": {\n      \"description\": \"Respond with **HTTP 200 OK** and `[accepted]` in the response body to [accept the webhook](https://docs.adyen.com/development-resources/webhooks#accept-notifications).\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-webhooks-account-notification-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountNotificationResponse
---
