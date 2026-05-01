---
description: The channel-specific configurations for the journey.
layout: schema
name: JourneyChannelSettings
properties_list:
- description: ''
  name: ConnectCampaignArn
  type: object
- description: ''
  name: ConnectCampaignExecutionRoleArn
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-journey-channel-settings-schema.json
slug: amazon-pinpoint-journey-channel-settings
source_filename: amazon-pinpoint-journey-channel-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-channel-settings-schema.json\",\n  \"title\": \"JourneyChannelSettings\",\n  \"description\": \"The channel-specific configurations for the journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectCampaignArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of the Connect Campaign.\"\n        }\n      ]\n    },\n    \"ConnectCampaignExecutionRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"IAM role ARN to be assumed when invoking Connect campaign execution APIs for dialing.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-channel-settings-schema.json
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
title: JourneyChannelSettings
---
