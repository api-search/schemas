---
description: Text config for Message Header.
layout: schema
name: InAppMessageHeaderConfig
properties_list:
- description: ''
  name: Alignment
  type: object
- description: ''
  name: Header
  type: object
- description: ''
  name: TextColor
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-in-app-message-header-config-schema.json
slug: amazon-pinpoint-in-app-message-header-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-message-header-config-schema.json\",\n  \"title\": \"InAppMessageHeaderConfig\",\n  \"description\": \"Text config for Message Header.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Alignment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Alignment\"\n        },\n        {\n          \"description\": \"The alignment of the text. Valid values: LEFT, CENTER, RIGHT.\"\n        }\n      ]\n    },\n    \"Header\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Message Header.\"\n        }\n      ]\n    },\n    \"TextColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\"\
  : \"The text color.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Alignment\",\n    \"Header\",\n    \"TextColor\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-message-header-config-schema.json
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
title: InAppMessageHeaderConfig
---
