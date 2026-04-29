---
description: Response containing disconnect order details
layout: schema
name: DisconnectResponse
properties_list:
- description: The unique identifier for the disconnect order
  name: orderId
  type: string
- description: The current status of the disconnect order
  name: orderStatus
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-disconnect-response-schema.json
slug: phone-numbers-disconnect-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-disconnect-response-schema.json\",\n  \"title\": \"DisconnectResponse\",\n  \"description\": \"Response containing disconnect order details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the disconnect order\"\n    },\n    \"orderStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the disconnect order\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-disconnect-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: DisconnectResponse
---
