---
description: DeliveryTime schema from AhaSend API
layout: schema
name: DeliveryTime
properties_list:
- description: The recipient domain
  name: recipient_domain
  type: string
- description: The average time from reception to delivery in seconds
  name: delivery_time
  type: number
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-delivery-time-schema.json
slug: openapi-v2-delivery-time
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-delivery-time-schema.json\",\n  \"title\": \"DeliveryTime\",\n  \"description\": \"DeliveryTime schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recipient_domain\": {\n      \"type\": \"string\",\n      \"format\": \"fqdn\",\n      \"description\": \"The recipient domain\",\n      \"example\": \"mail.example.com\"\n    },\n    \"delivery_time\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The average time from reception to delivery in seconds\",\n      \"example\": 1.0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-delivery-time-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: DeliveryTime
---
