---
description: Message schema from Adyen API
layout: schema
name: Message
properties_list:
- description: The message code.
  name: code
  type: string
- description: The message text.
  name: text
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-message-schema.json
slug: notifications-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-message-schema.json\",\n  \"title\": \"Message\",\n  \"description\": \"Message schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"description\": \"The message code.\",\n      \"type\": \"string\"\n    },\n    \"text\": {\n      \"description\": \"The message text.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-message-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Message
---
