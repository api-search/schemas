---
description: DeliveryInfo schema from AT&T API
layout: schema
name: DeliveryInfo
properties_list:
- description: Recipient phone number
  name: address
  type: string
- description: Current delivery status of the message
  name: deliveryStatus
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/sms-api-delivery-info-schema.json
slug: sms-api-delivery-info
source_filename: sms-api-delivery-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-delivery-info-schema.json\",\n  \"title\": \"DeliveryInfo\",\n  \"description\": \"DeliveryInfo schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Recipient phone number\",\n      \"example\": \"tel:+12125551234\"\n    },\n    \"deliveryStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current delivery status of the message\",\n      \"enum\": [\n        \"DeliveredToNetwork\",\n        \"DeliveredToTerminal\",\n        \"DeliveryImpossible\",\n        \"MessageWaiting\",\n        \"DeliveryUncertain\"\n      ],\n      \"example\": \"DeliveredToTerminal\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-delivery-info-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: DeliveryInfo
---
