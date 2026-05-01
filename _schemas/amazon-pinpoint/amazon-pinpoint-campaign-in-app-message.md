---
description: In-app message configuration.
layout: schema
name: CampaignInAppMessage
properties_list:
- description: ''
  name: Body
  type: object
- description: ''
  name: Content
  type: object
- description: ''
  name: CustomConfig
  type: object
- description: ''
  name: Layout
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-campaign-in-app-message-schema.json
slug: amazon-pinpoint-campaign-in-app-message
source_filename: amazon-pinpoint-campaign-in-app-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-in-app-message-schema.json\",\n  \"title\": \"CampaignInAppMessage\",\n  \"description\": \"In-app message configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The message body of the notification, the email body or the text message.\"\n        }\n      ]\n    },\n    \"Content\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfInAppMessageContent\"\n        },\n        {\n          \"description\": \"In-app message content.\"\n        }\n      ]\n    },\n    \"CustomConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n\
  \        {\n          \"description\": \"Custom config to be sent to client.\"\n        }\n      ]\n    },\n    \"Layout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Layout\"\n        },\n        {\n          \"description\": \"In-app message layout.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-in-app-message-schema.json
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
title: CampaignInAppMessage
---
