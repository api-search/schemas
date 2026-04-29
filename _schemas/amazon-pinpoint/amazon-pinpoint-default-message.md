---
description: Specifies the default message for all channels.
layout: schema
name: DefaultMessage
properties_list:
- description: ''
  name: Body
  type: object
- description: ''
  name: Substitutions
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-default-message-schema.json
slug: amazon-pinpoint-default-message
source_filename: amazon-pinpoint-default-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-default-message-schema.json\",\n  \"title\": \"DefaultMessage\",\n  \"description\": \"Specifies the default message for all channels.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The default body of the message.\"\n        }\n      ]\n    },\n    \"Substitutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOf__string\"\n        },\n        {\n          \"description\": \"The default message variables to use in the message. You can override these default variables with individual address variables.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-default-message-schema.json
tags:
- AWS
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
title: DefaultMessage
---
