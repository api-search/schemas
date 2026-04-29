---
description: ''
layout: schema
name: MessageResponseBlock
properties_list:
- description: Unique identifier of the message sender.
  name: initiatingPartyId
  type: string
- description: A point-to-point unique identifier is assigned to every message by the message initiator.
  name: messageId
  type: string
- description: ISO 8601 format date and time in Coordinated Universal Time (UTC) when this message was created.
  name: creationDateTime
  type: string
- description: Original message identifier generated and sent by the initiator of the request message.
  name: originalMessageId
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-message-response-block-schema.json
slug: mastercard-debtor-service-provider-resources-message-response-block
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageResponseBlock\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"initiatingPartyId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the message sender.\"\n    },\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"A point-to-point unique identifier is assigned to every message by the message initiator.\"\n    },\n    \"creationDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 format date and time in Coordinated Universal Time (UTC) when this message was created.\"\n    },\n    \"originalMessageId\": {\n      \"type\": \"string\",\n      \"description\": \"Original message identifier generated and sent by the initiator of the request message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-message-response-block-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: MessageResponseBlock
---
