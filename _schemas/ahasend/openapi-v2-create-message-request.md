---
description: CreateMessageRequest schema from AhaSend API
layout: schema
name: CreateMessageRequest
properties_list:
- description: ''
  name: from
  type: object
- description: This does not set the To header to multiple addresses, it sends a separate message for each recipient
  name: recipients
  type: array
- description: If provided, the reply-to header in headers array must not be provided
  name: reply_to
  type: object
- description: Email subject line
  name: subject
  type: string
- description: Plain text content. Required if html_content is empty
  name: text_content
  type: string
- description: HTML content. Required if text_content is empty
  name: html_content
  type: string
- description: AMP HTML content
  name: amp_content
  type: string
- description: File attachments
  name: attachments
  type: array
- description: Custom email headers. reply-to header cannot be provided if reply_to is provided, message-id will be ignored and automatically generated
  name: headers
  type: object
- description: Global substitutions, recipient substitutions override global
  name: substitutions
  type: object
- description: Tags for categorizing messages
  name: tags
  type: array
- description: If true, the message will be sent to the sandbox environment
  name: sandbox
  type: boolean
- description: The result of the sandbox send
  name: sandbox_result
  type: string
- description: Tracking settings for the message, overrides default account settings
  name: tracking
  type: object
- description: Retention settings for the message, overrides default account settings
  name: retention
  type: object
- description: Schedule for message delivery
  name: schedule
  type: object
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-create-message-request-schema.json
slug: openapi-v2-create-message-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-message-request-schema.json\",\n  \"title\": \"CreateMessageRequest\",\n  \"description\": \"CreateMessageRequest schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"recipients\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Recipient\"\n      },\n      \"minItems\": 1,\n      \"description\": \"This does not set the To header to multiple addresses, it sends a separate message for each recipient\",\n      \"example\": [\n        {\n          \"email\": \"user@example.com\",\n          \"name\": \"Example Name\",\n          \"substitutions\": {}\n        }\n      ]\n    },\n    \"reply_to\": {\n      \"$ref\": \"#/components/schemas/Address\",\n\
  \      \"description\": \"If provided, the reply-to header in headers array must not be provided\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Email subject line\",\n      \"example\": \"example_value\"\n    },\n    \"text_content\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text content. Required if html_content is empty\",\n      \"example\": \"example_value\"\n    },\n    \"html_content\": {\n      \"type\": \"string\",\n      \"description\": \"HTML content. Required if text_content is empty\",\n      \"example\": \"example_value\"\n    },\n    \"amp_content\": {\n      \"type\": \"string\",\n      \"description\": \"AMP HTML content\",\n      \"example\": \"example_value\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Attachment\"\n      },\n      \"description\": \"File attachments\",\n      \"example\": [\n        {\n          \"base64\": true,\n\
  \          \"data\": \"example_value\",\n          \"content_type\": \"example_value\",\n          \"content_disposition\": \"example_value\",\n          \"content_id\": \"500123\"\n        }\n      ]\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom email headers. reply-to header cannot be provided if reply_to is provided, message-id will be ignored and automatically generated\",\n      \"example\": {}\n    },\n    \"substitutions\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Global substitutions, recipient substitutions override global\",\n      \"example\": {}\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags for categorizing messages\",\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"sandbox\": {\n \
  \     \"type\": \"boolean\",\n      \"description\": \"If true, the message will be sent to the sandbox environment\",\n      \"default\": false,\n      \"example\": true\n    },\n    \"sandbox_result\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"deliver\",\n        \"bounce\",\n        \"defer\",\n        \"fail\",\n        \"suppress\"\n      ],\n      \"description\": \"The result of the sandbox send\",\n      \"example\": \"deliver\"\n    },\n    \"tracking\": {\n      \"$ref\": \"#/components/schemas/Tracking\",\n      \"description\": \"Tracking settings for the message, overrides default account settings\"\n    },\n    \"retention\": {\n      \"$ref\": \"#/components/schemas/Retention\",\n      \"description\": \"Retention settings for the message, overrides default account settings\"\n    },\n    \"schedule\": {\n      \"$ref\": \"#/components/schemas/MessageSchedule\",\n      \"description\": \"Schedule for message delivery\"\n    }\n  },\n  \"required\": [\n\
  \    \"from\",\n    \"recipients\",\n    \"subject\"\n  ],\n  \"example\": {\n    \"from\": {\n      \"email\": \"noreply@example.com\",\n      \"name\": \"Example Corp\"\n    },\n    \"recipients\": [\n      {\n        \"email\": \"user@example.com\",\n        \"name\": \"John Doe\"\n      }\n    ],\n    \"subject\": \"Welcome to Example Corp\",\n    \"html_content\": \"<h1>Welcome {{first_name}}!</h1>\",\n    \"text_content\": \"Welcome {{first_name}}!\",\n    \"substitutions\": {\n      \"first_name\": \"John\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-message-request-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: CreateMessageRequest
---
