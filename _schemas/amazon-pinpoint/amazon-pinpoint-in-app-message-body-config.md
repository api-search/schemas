---
description: Text config for Message Body.
layout: schema
name: InAppMessageBodyConfig
properties_list:
- description: ''
  name: Alignment
  type: object
- description: ''
  name: Body
  type: object
- description: ''
  name: TextColor
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-in-app-message-body-config-schema.json
slug: amazon-pinpoint-in-app-message-body-config
source_filename: amazon-pinpoint-in-app-message-body-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-message-body-config-schema.json\",\n  \"title\": \"InAppMessageBodyConfig\",\n  \"description\": \"Text config for Message Body.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Alignment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Alignment\"\n        },\n        {\n          \"description\": \"The alignment of the text. Valid values: LEFT, CENTER, RIGHT.\"\n        }\n      ]\n    },\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Message Body.\"\n        }\n      ]\n    },\n    \"TextColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\"\
  : \"The text color.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Alignment\",\n    \"TextColor\",\n    \"Body\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-message-body-config-schema.json
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
title: InAppMessageBodyConfig
---
