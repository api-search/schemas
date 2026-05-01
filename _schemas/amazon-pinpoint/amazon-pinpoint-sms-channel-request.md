---
description: Specifies the status and settings of the SMS channel for an application.
layout: schema
name: SMSChannelRequest
properties_list:
- description: ''
  name: Enabled
  type: object
- description: ''
  name: SenderId
  type: object
- description: ''
  name: ShortCode
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-sms-channel-request-schema.json
slug: amazon-pinpoint-sms-channel-request
source_filename: amazon-pinpoint-sms-channel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-sms-channel-request-schema.json\",\n  \"title\": \"SMSChannelRequest\",\n  \"description\": \"Specifies the status and settings of the SMS channel for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether to enable the SMS channel for the application.\"\n        }\n      ]\n    },\n    \"SenderId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The identity that you want to display on recipients' devices when they receive messages from the SMS channel.\"\n        }\n      ]\n    },\n    \"ShortCode\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The registered short code that you want to use when you send messages through the SMS channel.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-sms-channel-request-schema.json
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
title: SMSChannelRequest
---
