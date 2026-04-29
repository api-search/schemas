---
description: AchNotificationOfChangeNotificationRequest schema from Adyen API
layout: schema
name: AchNotificationOfChangeNotificationRequest
properties_list:
- description: Timestamp for when the webhook was created.
  name: createdAt
  type: string
- description: Contains details of the update.
  name: data
  type: object
- description: 'The environment from which the webhook originated. Possible values: **test**, **live**.'
  name: environment
  type: string
- description: Type of notification.
  name: type
  type: string
- description: The version of this webhook type.
  name: version
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/webhooks-ach-notification-of-change-notification-request-schema.json
slug: webhooks-ach-notification-of-change-notification-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-ach-notification-of-change-notification-request-schema.json\",\n  \"title\": \"AchNotificationOfChangeNotificationRequest\",\n  \"description\": \"AchNotificationOfChangeNotificationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"description\": \"Timestamp for when the webhook was created.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"data\": {\n      \"description\": \"Contains details of the update.\",\n      \"$ref\": \"#/components/schemas/AchNotificationOfChangeNotificationRequestData\"\n    },\n    \"environment\": {\n      \"description\": \"The environment from which the webhook originated.\\n\\nPossible values: **test**, **live**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\"\
  : \"Type of notification.\",\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"description\": \"The version of this webhook type.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"createdAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-ach-notification-of-change-notification-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AchNotificationOfChangeNotificationRequest
---
