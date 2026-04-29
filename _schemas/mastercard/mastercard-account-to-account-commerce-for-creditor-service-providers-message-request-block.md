---
description: ''
layout: schema
name: MessageRequestBlock
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
- description: Unique identifier assigned by Mastercard to define the commercial product construct. * Refer to Codes and Formats section for more details.
  name: businessType
  type: number
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-message-request-block-schema.json
slug: mastercard-account-to-account-commerce-for-creditor-service-providers-message-request-block
source_filename: mastercard-account-to-account-commerce-for-creditor-service-providers-message-request-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageRequestBlock\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"initiatingPartyId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the message sender.\"\n    },\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"A point-to-point unique identifier is assigned to every message by the message initiator.\"\n    },\n    \"creationDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 format date and time in Coordinated Universal Time (UTC) when this message was created.\"\n    },\n    \"businessType\": {\n      \"type\": \"number\",\n      \"description\": \"Unique identifier assigned by Mastercard to define the commercial product construct. * Refer to Codes and Formats section for more details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-message-request-block-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: MessageRequestBlock
---
