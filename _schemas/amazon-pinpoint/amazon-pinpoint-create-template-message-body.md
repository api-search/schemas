---
description: Provides information about a request to create a message template.
layout: schema
name: CreateTemplateMessageBody
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: RequestID
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-create-template-message-body-schema.json
slug: amazon-pinpoint-create-template-message-body
source_filename: amazon-pinpoint-create-template-message-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-create-template-message-body-schema.json\",\n  \"title\": \"CreateTemplateMessageBody\",\n  \"description\": \"Provides information about a request to create a message template.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the message template that was created.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The message that's returned from the API for the request to create the message template.\"\n        }\n      ]\n    },\n    \"RequestID\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the request to create the message template.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-create-template-message-body-schema.json
tags:
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: CreateTemplateMessageBody
---
