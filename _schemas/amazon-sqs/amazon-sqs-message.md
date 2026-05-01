---
description: An Amazon SQS message
layout: schema
name: Message
properties_list:
- description: A unique identifier for the message
  name: MessageId
  type: string
- description: An identifier associated with the act of receiving the message. A new receipt handle is returned every time you receive a message. When deleting a message, you provide the last received receipt handle
  name: ReceiptHandle
  type: string
- description: An MD5 digest of the non-URL-encoded message body string
  name: MD5OfBody
  type: string
- description: The message's contents (not URL-encoded)
  name: Body
  type: string
- description: A map of the attributes requested in ReceiveMessage to their respective values.
  name: Attribute
  type: array
- description: Each message attribute consists of a Name, Type, and Value.
  name: MessageAttribute
  type: array
provider_name: Amazon SQS
provider_slug: amazon-sqs
schema_file: json-schema/amazon-sqs-message-schema.json
slug: amazon-sqs-message
source_filename: amazon-sqs-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Message\",\n  \"type\": \"object\",\n  \"description\": \"An Amazon SQS message\",\n  \"properties\": {\n    \"MessageId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the message\"\n    },\n    \"ReceiptHandle\": {\n      \"type\": \"string\",\n      \"description\": \"An identifier associated with the act of receiving the message. A new receipt handle is returned every time you receive a message. When deleting a message, you provide the last received receipt handle to delete the message.\"\n    },\n    \"MD5OfBody\": {\n      \"type\": \"string\",\n      \"description\": \"An MD5 digest of the non-URL-encoded message body string\"\n    },\n    \"Body\": {\n      \"type\": \"string\",\n      \"description\": \"The message's contents (not URL-encoded)\"\n    },\n    \"Attribute\": {\n      \"type\": \"array\",\n      \"description\": \"A map of the attributes\
  \ requested in ReceiveMessage to their respective values.\"\n    },\n    \"MessageAttribute\": {\n      \"type\": \"array\",\n      \"description\": \"Each message attribute consists of a Name, Type, and Value.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sqs/refs/heads/main/json-schema/amazon-sqs-message-schema.json
tags:
- Cloud
- Distributed Systems
- Messaging
- Microservices
- Queue
title: Message
---
