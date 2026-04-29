---
description: Specifies the "From" address for an email message that's sent to participants in a journey.
layout: schema
name: JourneyEmailMessage
properties_list:
- description: ''
  name: FromAddress
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-journey-email-message-schema.json
slug: amazon-pinpoint-journey-email-message
source_filename: amazon-pinpoint-journey-email-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-email-message-schema.json\",\n  \"title\": \"JourneyEmailMessage\",\n  \"description\": \"Specifies the \\\"From\\\" address for an email message that's sent to participants in a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FromAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The verified email address to send the email message from. The default address is the FromAddress specified for the email channel for the application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-email-message-schema.json
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
title: JourneyEmailMessage
---
