---
description: Button Config for an in-app message.
layout: schema
name: InAppMessageButton
properties_list:
- description: ''
  name: Android
  type: object
- description: ''
  name: DefaultConfig
  type: object
- description: ''
  name: IOS
  type: object
- description: ''
  name: Web
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-in-app-message-button-schema.json
slug: amazon-pinpoint-in-app-message-button
source_filename: amazon-pinpoint-in-app-message-button-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-message-button-schema.json\",\n  \"title\": \"InAppMessageButton\",\n  \"description\": \"Button Config for an in-app message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Android\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OverrideButtonConfiguration\"\n        },\n        {\n          \"description\": \"Default button content.\"\n        }\n      ]\n    },\n    \"DefaultConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultButtonConfiguration\"\n        },\n        {\n          \"description\": \"Default button content.\"\n        }\n      ]\n    },\n    \"IOS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OverrideButtonConfiguration\"\n        },\n        {\n\
  \          \"description\": \"Default button content.\"\n        }\n      ]\n    },\n    \"Web\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OverrideButtonConfiguration\"\n        },\n        {\n          \"description\": \"Default button content.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-message-button-schema.json
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
title: InAppMessageButton
---
