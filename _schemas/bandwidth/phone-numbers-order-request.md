---
description: Request to order phone numbers
layout: schema
name: OrderRequest
properties_list:
- description: A name for the order (required, max 50 characters)
  name: name
  type: string
- description: The site to assign the numbers to
  name: siteId
  type: string
- description: The SIP peer to assign the numbers to
  name: peerId
  type: string
- description: ''
  name: existingTelephoneNumberOrderType
  type: object
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-order-request-schema.json
slug: phone-numbers-order-request
source_filename: phone-numbers-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-order-request-schema.json\",\n  \"title\": \"OrderRequest\",\n  \"description\": \"Request to order phone numbers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\": \"A name for the order (required, max 50 characters)\"\n    },\n    \"siteId\": {\n      \"type\": \"string\",\n      \"description\": \"The site to assign the numbers to\"\n    },\n    \"peerId\": {\n      \"type\": \"string\",\n      \"description\": \"The SIP peer to assign the numbers to\"\n    },\n    \"existingTelephoneNumberOrderType\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"telephoneNumberList\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n  \
  \        \"description\": \"List of specific phone numbers to order\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-order-request-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: OrderRequest
---
