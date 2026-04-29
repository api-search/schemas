---
description: The configuration for the message content.
layout: schema
name: InAppMessageContent
properties_list:
- description: ''
  name: BackgroundColor
  type: object
- description: ''
  name: BodyConfig
  type: object
- description: ''
  name: HeaderConfig
  type: object
- description: ''
  name: ImageUrl
  type: object
- description: ''
  name: PrimaryBtn
  type: object
- description: ''
  name: SecondaryBtn
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-in-app-message-content-schema.json
slug: amazon-pinpoint-in-app-message-content
source_filename: amazon-pinpoint-in-app-message-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-message-content-schema.json\",\n  \"title\": \"InAppMessageContent\",\n  \"description\": \"The configuration for the message content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BackgroundColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The background color for the message.\"\n        }\n      ]\n    },\n    \"BodyConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppMessageBodyConfig\"\n        },\n        {\n          \"description\": \"The configuration for the message body.\"\n        }\n      ]\n    },\n    \"HeaderConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppMessageHeaderConfig\"\
  \n        },\n        {\n          \"description\": \"The configuration for the message header.\"\n        }\n      ]\n    },\n    \"ImageUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The image url for the background of message.\"\n        }\n      ]\n    },\n    \"PrimaryBtn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppMessageButton\"\n        },\n        {\n          \"description\": \"The first button inside the message.\"\n        }\n      ]\n    },\n    \"SecondaryBtn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppMessageButton\"\n        },\n        {\n          \"description\": \"The second button inside message.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-message-content-schema.json
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
title: InAppMessageContent
---
