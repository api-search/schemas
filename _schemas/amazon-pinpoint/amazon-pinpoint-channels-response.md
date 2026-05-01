---
description: Provides information about the general settings and status of all channels for an application, including channels that aren't enabled for the application.
layout: schema
name: ChannelsResponse
properties_list:
- description: ''
  name: Channels
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-channels-response-schema.json
slug: amazon-pinpoint-channels-response
source_filename: amazon-pinpoint-channels-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-channels-response-schema.json\",\n  \"title\": \"ChannelsResponse\",\n  \"description\": \"Provides information about the general settings and status of all channels for an application, including channels that aren't enabled for the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfChannelResponse\"\n        },\n        {\n          \"description\": \"A map that contains a multipart response for each channel. For each item in this object, the ChannelType is the key and the Channel is the value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Channels\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-channels-response-schema.json
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
title: ChannelsResponse
---
