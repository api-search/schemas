---
description: ExpireNotificationRequest schema from Adyen API
layout: schema
name: ExpireNotificationRequest
properties_list:
- description: Informs about the origin of the notification. The value is **true** when originating from the live environment, **false** for the test environment.
  name: live
  type: string
- description: A container object for the details included in the notification.
  name: notificationItems
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/webhooks-expire-notification-request-schema.json
slug: webhooks-expire-notification-request
source_filename: webhooks-expire-notification-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-expire-notification-request-schema.json\",\n  \"title\": \"ExpireNotificationRequest\",\n  \"description\": \"ExpireNotificationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"live\": {\n      \"description\": \"Informs about the origin of the notification. The value is **true** when originating from the live environment, **false** for the test environment.\",\n      \"type\": \"string\"\n    },\n    \"notificationItems\": {\n      \"description\": \"A container object for the details included in the notification.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ExpireNotificationRequestItemWrapper\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-expire-notification-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ExpireNotificationRequest
---
