---
description: Specifies the status and settings of the ADM (Amazon Device Messaging) channel for an application.
layout: schema
name: ADMChannelRequest
properties_list:
- description: ''
  name: ClientId
  type: object
- description: ''
  name: ClientSecret
  type: object
- description: ''
  name: Enabled
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-adm-channel-request-schema.json
slug: amazon-pinpoint-adm-channel-request
source_filename: amazon-pinpoint-adm-channel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-adm-channel-request-schema.json\",\n  \"title\": \"ADMChannelRequest\",\n  \"description\": \"Specifies the status and settings of the ADM (Amazon Device Messaging) channel for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Client ID that you received from Amazon to send messages by using ADM.\"\n        }\n      ]\n    },\n    \"ClientSecret\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Client Secret that you received from Amazon to send messages by using ADM.\"\n        }\n      ]\n    },\n    \"Enabled\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether to enable the ADM channel for the application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClientSecret\",\n    \"ClientId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-adm-channel-request-schema.json
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
title: ADMChannelRequest
---
