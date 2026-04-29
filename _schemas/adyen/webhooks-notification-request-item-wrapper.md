---
description: NotificationRequestItemWrapper schema from Adyen API
layout: schema
name: NotificationRequestItemWrapper
properties_list:
- description: ''
  name: NotificationRequestItem
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/webhooks-notification-request-item-wrapper-schema.json
slug: webhooks-notification-request-item-wrapper
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-notification-request-item-wrapper-schema.json\",\n  \"title\": \"NotificationRequestItemWrapper\",\n  \"description\": \"NotificationRequestItemWrapper schema from Adyen API\",\n  \"properties\": {\n    \"NotificationRequestItem\": {\n      \"$ref\": \"#/components/schemas/NotificationRequestItem\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-notification-request-item-wrapper-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NotificationRequestItemWrapper
---
