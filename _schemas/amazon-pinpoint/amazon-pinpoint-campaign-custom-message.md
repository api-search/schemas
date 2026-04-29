---
description: Specifies the contents of a message that's sent through a custom channel to recipients of a campaign.
layout: schema
name: CampaignCustomMessage
properties_list:
- description: ''
  name: Data
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-campaign-custom-message-schema.json
slug: amazon-pinpoint-campaign-custom-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-custom-message-schema.json\",\n  \"title\": \"CampaignCustomMessage\",\n  \"description\": \"Specifies the contents of a message that's sent through a custom channel to recipients of a campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The raw, JSON-formatted string to use as the payload for the message. The maximum size is 5 KB.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-custom-message-schema.json
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
title: CampaignCustomMessage
---
