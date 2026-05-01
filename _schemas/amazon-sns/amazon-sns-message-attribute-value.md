---
description: ''
layout: schema
name: MessageAttributeValue
properties_list:
- description: The data type of the attribute. Supported types are String, String.Array, Number, and Binary.
  name: DataType
  type: string
- description: The string value of the attribute
  name: StringValue
  type: string
- description: The binary (base64-encoded) value of the attribute
  name: BinaryValue
  type: string
provider_name: Amazon SNS
provider_slug: amazon-sns
schema_file: json-schema/amazon-sns-message-attribute-value-schema.json
slug: amazon-sns-message-attribute-value
source_filename: amazon-sns-message-attribute-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageAttributeValue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataType\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the attribute. Supported types are String, String.Array, Number, and Binary.\"\n    },\n    \"StringValue\": {\n      \"type\": \"string\",\n      \"description\": \"The string value of the attribute\"\n    },\n    \"BinaryValue\": {\n      \"type\": \"string\",\n      \"description\": \"The binary (base64-encoded) value of the attribute\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/json-schema/amazon-sns-message-attribute-value-schema.json
tags:
- Email
- Messaging
- Notifications
- Pub/Sub
- Push Notifications
- SMS
title: MessageAttributeValue
---
