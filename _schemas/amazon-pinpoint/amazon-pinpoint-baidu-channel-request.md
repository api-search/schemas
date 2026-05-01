---
description: Specifies the status and settings of the Baidu (Baidu Cloud Push) channel for an application.
layout: schema
name: BaiduChannelRequest
properties_list:
- description: ''
  name: ApiKey
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: SecretKey
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-baidu-channel-request-schema.json
slug: amazon-pinpoint-baidu-channel-request
source_filename: amazon-pinpoint-baidu-channel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-baidu-channel-request-schema.json\",\n  \"title\": \"BaiduChannelRequest\",\n  \"description\": \"Specifies the status and settings of the Baidu (Baidu Cloud Push) channel for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApiKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The API key that you received from the Baidu Cloud Push service to communicate with the service.\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether to enable the Baidu channel for the application.\"\n        }\n      ]\n    },\n    \"SecretKey\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The secret key that you received from the Baidu Cloud Push service to communicate with the service.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SecretKey\",\n    \"ApiKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-baidu-channel-request-schema.json
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
title: BaiduChannelRequest
---
