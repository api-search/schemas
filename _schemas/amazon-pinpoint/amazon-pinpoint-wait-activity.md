---
description: Specifies the settings for a wait activity in a journey. This type of activity waits for a certain amount of time or until a specific date and time before moving participants to the next activity in a journey.
layout: schema
name: WaitActivity
properties_list:
- description: ''
  name: NextActivity
  type: object
- description: ''
  name: WaitTime
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-wait-activity-schema.json
slug: amazon-pinpoint-wait-activity
source_filename: amazon-pinpoint-wait-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-wait-activity-schema.json\",\n  \"title\": \"WaitActivity\",\n  \"description\": \"Specifies the settings for a wait activity in a journey. This type of activity waits for a certain amount of time or until a specific date and time before moving participants to the next activity in a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextActivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the next activity to perform, after performing the wait activity.\"\n        }\n      ]\n    },\n    \"WaitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WaitTime\"\n        },\n        {\n          \"description\": \"The amount\
  \ of time to wait or the date and time when the activity moves participants to the next activity in the journey.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-wait-activity-schema.json
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
title: WaitActivity
---
