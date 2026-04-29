---
description: Get in-app messages response object.
layout: schema
name: InAppMessagesResponse
properties_list:
- description: ''
  name: InAppMessageCampaigns
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-in-app-messages-response-schema.json
slug: amazon-pinpoint-in-app-messages-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-messages-response-schema.json\",\n  \"title\": \"InAppMessagesResponse\",\n  \"description\": \"Get in-app messages response object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InAppMessageCampaigns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfInAppMessageCampaign\"\n        },\n        {\n          \"description\": \"List of targeted in-app message campaigns.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-messages-response-schema.json
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
title: InAppMessagesResponse
---
