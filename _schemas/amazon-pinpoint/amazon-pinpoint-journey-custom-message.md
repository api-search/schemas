---
description: Specifies the message content for a custom channel message that's sent to participants in a journey.
layout: schema
name: JourneyCustomMessage
properties_list:
- description: ''
  name: Data
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-journey-custom-message-schema.json
slug: amazon-pinpoint-journey-custom-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-custom-message-schema.json\",\n  \"title\": \"JourneyCustomMessage\",\n  \"description\": \"Specifies the message content for a custom channel message that's sent to participants in a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The message content that's passed to an AWS Lambda function or to a web hook.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-custom-message-schema.json
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
title: JourneyCustomMessage
---
