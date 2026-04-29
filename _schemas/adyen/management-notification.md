---
description: Notification schema from Adyen API
layout: schema
name: Notification
properties_list:
- description: The type of event notification sent when you select the notification button.
  name: category
  type: string
- description: The text shown in the prompt which opens when you select the notification button. For example, the description of the input box for pay-at-table.
  name: details
  type: string
- description: Enables sending event notifications either by pressing the Confirm key on terminals with a keypad or by tapping the event notification button on the terminal screen.
  name: enabled
  type: boolean
- description: Shows or hides the event notification button on the screen of terminal models that have a keypad.
  name: showButton
  type: boolean
- description: The name of the notification button on the terminal screen.
  name: title
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-notification-schema.json
slug: management-notification
source_filename: management-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-notification-schema.json\",\n  \"title\": \"Notification\",\n  \"description\": \"Notification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"description\": \"The type of event notification sent when you select the notification button.\",\n      \"enum\": [\n        \"SaleWakeUp\",\n        \"KeyPressed\"\n      ],\n      \"type\": \"string\"\n    },\n    \"details\": {\n      \"description\": \"The text shown in the prompt which opens when you select the notification button. For example, the description of the input box for pay-at-table.\",\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"description\": \"Enables sending event notifications either by pressing the Confirm key on terminals with a keypad or by tapping the event notification\
  \ button on the terminal screen.\",\n      \"type\": \"boolean\"\n    },\n    \"showButton\": {\n      \"description\": \"Shows or hides the event notification button on the screen of terminal models that have a keypad.\",\n      \"type\": \"boolean\"\n    },\n    \"title\": {\n      \"description\": \"The name of the notification button on the terminal screen.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-notification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Notification
---
