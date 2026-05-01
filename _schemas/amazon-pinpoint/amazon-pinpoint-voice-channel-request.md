---
description: Specifies the status and settings of the voice channel for an application.
layout: schema
name: VoiceChannelRequest
properties_list:
- description: ''
  name: Enabled
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-voice-channel-request-schema.json
slug: amazon-pinpoint-voice-channel-request
source_filename: amazon-pinpoint-voice-channel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-voice-channel-request-schema.json\",\n  \"title\": \"VoiceChannelRequest\",\n  \"description\": \"Specifies the status and settings of the voice channel for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether to enable the voice channel for the application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-voice-channel-request-schema.json
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
title: VoiceChannelRequest
---
