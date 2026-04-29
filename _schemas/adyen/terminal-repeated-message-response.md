---
description: RepeatedMessageResponse schema from Adyen API
layout: schema
name: RepeatedMessageResponse
properties_list:
- description: ''
  name: MessageHeader
  type: object
- description: ''
  name: RepeatedResponseMessageBody
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-repeated-message-response-schema.json
slug: terminal-repeated-message-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-repeated-message-response-schema.json\",\n  \"title\": \"RepeatedMessageResponse\",\n  \"description\": \"RepeatedMessageResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MessageHeader\": {\n      \"$ref\": \"#/components/schemas/MessageHeader\"\n    },\n    \"RepeatedResponseMessageBody\": {\n      \"$ref\": \"#/components/schemas/RepeatedResponseMessageBody\"\n    }\n  },\n  \"required\": [\n    \"MessageHeader\",\n    \"RepeatedResponseMessageBody\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-repeated-message-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RepeatedMessageResponse
---
