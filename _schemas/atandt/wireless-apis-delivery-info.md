---
description: SMS delivery status information
layout: schema
name: Delivery Info
properties_list:
- description: ''
  name: address
  type: string
- description: ''
  name: deliveryStatus
  type: string
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/wireless-apis-delivery-info-schema.json
slug: wireless-apis-delivery-info
source_filename: wireless-apis-delivery-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/wireless/delivery-info\",\n  \"title\": \"Delivery Info\",\n  \"description\": \"SMS delivery status information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\"\n    },\n    \"deliveryStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DeliveredToTerminal\",\n        \"DeliveryImpossible\",\n        \"DeliveredToNetwork\",\n        \"MessageWaiting\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/wireless-apis-delivery-info-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Delivery Info
---
