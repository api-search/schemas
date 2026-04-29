---
description: A WhatsApp Business phone number.
layout: schema
name: WhatsAppPhoneNumber
properties_list:
- description: Phone number ID.
  name: id
  type: string
- description: Display phone number.
  name: display_phone_number
  type: string
- description: Verified business name.
  name: verified_name
  type: string
- description: Quality rating.
  name: quality_rating
  type: string
- description: Phone number status.
  name: status
  type: string
provider_name: Facebook
provider_slug: facebook
schema_file: json-schema/whatsapp-api-whatsapp-phone-number-schema.json
slug: whatsapp-api-whatsapp-phone-number
source_filename: whatsapp-api-whatsapp-phone-number-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/whatsapp-api-whatsapp-phone-number-schema.json\",\n  \"title\": \"WhatsAppPhoneNumber\",\n  \"description\": \"A WhatsApp Business phone number.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Phone number ID.\" },\n    \"display_phone_number\": { \"type\": \"string\", \"description\": \"Display phone number.\" },\n    \"verified_name\": { \"type\": \"string\", \"description\": \"Verified business name.\" },\n    \"quality_rating\": { \"type\": \"string\", \"description\": \"Quality rating.\", \"enum\": [\"GREEN\", \"YELLOW\", \"RED\"] },\n    \"status\": { \"type\": \"string\", \"description\": \"Phone number status.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/whatsapp-api-whatsapp-phone-number-schema.json
tags:
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
title: WhatsAppPhoneNumber
---
