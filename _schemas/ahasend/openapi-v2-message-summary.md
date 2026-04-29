---
description: MessageSummary schema from AhaSend API
layout: schema
name: MessageSummary
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: When the message was created
  name: created_at
  type: string
- description: When the message was last updated
  name: updated_at
  type: string
- description: When the message was sent
  name: sent_at
  type: string
- description: When the message was delivered
  name: delivered_at
  type: string
- description: When the message data will be purged
  name: retain_until
  type: string
- description: Message direction
  name: direction
  type: string
- description: Whether this is a bounce notification
  name: is_bounce_notification
  type: boolean
- description: Classification of bounce if applicable
  name: bounce_classification
  type: string
- description: List of delivery attempts for this message
  name: delivery_attempts
  type: array
- description: Message-ID header value
  name: message_id
  type: string
- description: API-generated message ID
  name: id
  type: string
- description: Message subject
  name: subject
  type: string
- description: Tags associated with the message
  name: tags
  type: array
- description: Sender email address
  name: sender
  type: string
- description: Recipient email address
  name: recipient
  type: string
- description: Current message status
  name: status
  type: string
- description: Number of delivery attempts
  name: num_attempts
  type: integer
- description: Number of clicks tracked for this message
  name: click_count
  type: integer
- description: Number of opens tracked for this message
  name: open_count
  type: integer
- description: ID of the original message (for bounce messages)
  name: reference_message_id
  type: integer
- description: Domain ID this message was sent from
  name: domain_id
  type: string
- description: Account ID this message belongs to
  name: account_id
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-message-summary-schema.json
slug: openapi-v2-message-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-summary-schema.json\",\n  \"title\": \"MessageSummary\",\n  \"description\": \"MessageSummary schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"message\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"message\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the message was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the message was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"sent_at\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"When the message was sent\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"delivered_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"When the message was delivered\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"retain_until\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the message data will be purged\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"incoming\",\n        \"outgoing\"\n      ],\n      \"description\": \"Message direction\",\n      \"example\": \"incoming\"\n    },\n    \"is_bounce_notification\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a bounce notification\",\n      \"example\": true\n    },\n    \"bounce_classification\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Classification of bounce if applicable\",\n      \"example\": \"example_value\"\n    },\n    \"delivery_attempts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DeliveryEvent\"\n      },\n      \"description\": \"List of delivery attempts for this message\",\n      \"example\": [\n        {\n          \"time\": \"2025-03-15T14:30:00Z\",\n          \"log\": \"example_value\",\n          \"status\": \"example_value\"\n        }\n      ]\n    },\n    \"message_id\": {\n      \"type\": \"string\",\n      \"description\": \"Message-ID header value\",\n      \"example\": \"500123\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"API-generated message ID\",\n      \"example\": \"500123\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Message subject\",\n      \"example\": \"example_value\"\n   \
  \ },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags associated with the message\",\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"sender\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Sender email address\",\n      \"example\": \"example_value\"\n    },\n    \"recipient\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Recipient email address\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current message status\",\n      \"example\": \"example_value\"\n    },\n    \"num_attempts\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of delivery attempts\",\n      \"example\": 1\n    },\n    \"click_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of clicks tracked for this message\"\
  ,\n      \"example\": 1\n    },\n    \"open_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of opens tracked for this message\",\n      \"example\": 1\n    },\n    \"reference_message_id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"ID of the original message (for bounce messages)\",\n      \"example\": 1\n    },\n    \"domain_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Domain ID this message was sent from\",\n      \"example\": \"500123\"\n    },\n    \"account_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Account ID this message belongs to\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"created_at\",\n    \"updated_at\",\n    \"retain_until\",\n    \"direction\",\n    \"is_bounce_notification\",\n    \"delivery_attempts\",\n    \"message_id\",\n    \"id\",\n    \"subject\",\n    \"\
  tags\",\n    \"sender\",\n    \"recipient\",\n    \"status\",\n    \"num_attempts\",\n    \"click_count\",\n    \"open_count\",\n    \"domain_id\",\n    \"account_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-message-summary-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: MessageSummary
---
