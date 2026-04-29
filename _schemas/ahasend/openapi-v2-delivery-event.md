---
description: DeliveryEvent schema from AhaSend API
layout: schema
name: DeliveryEvent
properties_list:
- description: Timestamp of the delivery event
  name: time
  type: string
- description: Log message for the delivery event
  name: log
  type: string
- description: Status of the delivery event
  name: status
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-delivery-event-schema.json
slug: openapi-v2-delivery-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-delivery-event-schema.json\",\n  \"title\": \"DeliveryEvent\",\n  \"description\": \"DeliveryEvent schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the delivery event\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"log\": {\n      \"type\": \"string\",\n      \"description\": \"Log message for the delivery event\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the delivery event\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"time\",\n    \"log\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-delivery-event-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: DeliveryEvent
---
