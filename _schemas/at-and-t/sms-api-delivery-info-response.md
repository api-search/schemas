---
description: DeliveryInfoResponse schema from AT&T API
layout: schema
name: DeliveryInfoResponse
properties_list:
- description: ''
  name: deliveryInfoList
  type: object
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/sms-api-delivery-info-response-schema.json
slug: sms-api-delivery-info-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-delivery-info-response-schema.json\",\n  \"title\": \"DeliveryInfoResponse\",\n  \"description\": \"DeliveryInfoResponse schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deliveryInfoList\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"deliveryInfo\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"address\": {\n                \"type\": \"string\",\n                \"description\": \"Recipient phone number\",\n                \"example\": \"tel:+12125551234\"\n              },\n              \"deliveryStatus\": {\n                \"type\": \"string\",\n                \"description\": \"Current delivery status of the message\",\n                \"enum\": [\n  \
  \                \"DeliveredToNetwork\",\n                  \"DeliveredToTerminal\",\n                  \"DeliveryImpossible\",\n                  \"MessageWaiting\",\n                  \"DeliveryUncertain\"\n                ],\n                \"example\": \"DeliveredToTerminal\"\n              }\n            }\n          }\n        },\n        \"resourceURL\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of this delivery info resource\",\n          \"example\": \"https://api.att.com/sms/v3/messaging/outbox/msg-500123\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-delivery-info-response-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: DeliveryInfoResponse
---
