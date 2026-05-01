---
description: InApp Template Request.
layout: schema
name: InAppTemplateRequest
properties_list:
- description: ''
  name: Content
  type: object
- description: ''
  name: CustomConfig
  type: object
- description: ''
  name: Layout
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: TemplateDescription
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-in-app-template-request-schema.json
slug: amazon-pinpoint-in-app-template-request
source_filename: amazon-pinpoint-in-app-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-template-request-schema.json\",\n  \"title\": \"InAppTemplateRequest\",\n  \"description\": \"InApp Template Request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Content\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfInAppMessageContent\"\n        },\n        {\n          \"description\": \"The content of the message, can include up to 5 modals. Each modal must contain a message, a header, and background color. ImageUrl and buttons are optional.\"\n        }\n      ]\n    },\n    \"CustomConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"Custom config to be sent to client.\"\n        }\n      ]\n    },\n    \"Layout\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Layout\"\n        },\n        {\n          \"description\": \"The layout of the message.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.\"\n        }\n      ]\n    },\n    \"TemplateDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The description of the template.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-template-request-schema.json
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
title: InAppTemplateRequest
---
