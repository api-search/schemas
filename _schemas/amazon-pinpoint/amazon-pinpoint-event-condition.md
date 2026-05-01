---
description: Specifies the conditions to evaluate for an event that applies to an activity in a journey.
layout: schema
name: EventCondition
properties_list:
- description: ''
  name: Dimensions
  type: object
- description: ''
  name: MessageActivity
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-event-condition-schema.json
slug: amazon-pinpoint-event-condition
source_filename: amazon-pinpoint-event-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-condition-schema.json\",\n  \"title\": \"EventCondition\",\n  \"description\": \"Specifies the conditions to evaluate for an event that applies to an activity in a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Dimensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventDimensions\"\n        },\n        {\n          \"description\": \"The dimensions for the event filter to use for the activity.\"\n        }\n      ]\n    },\n    \"MessageActivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The message identifier (message_id) for the message to use when determining whether message events meet the condition.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-condition-schema.json
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
title: EventCondition
---
