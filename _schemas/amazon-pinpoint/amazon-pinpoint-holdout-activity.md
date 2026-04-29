---
description: Specifies the settings for a holdout activity in a journey. This type of activity stops a journey for a specified percentage of participants.
layout: schema
name: HoldoutActivity
properties_list:
- description: ''
  name: NextActivity
  type: object
- description: ''
  name: Percentage
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-holdout-activity-schema.json
slug: amazon-pinpoint-holdout-activity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-holdout-activity-schema.json\",\n  \"title\": \"HoldoutActivity\",\n  \"description\": \"Specifies the settings for a holdout activity in a journey. This type of activity stops a journey for a specified percentage of participants.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextActivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the next activity to perform, after performing the holdout activity.\"\n        }\n      ]\n    },\n    \"Percentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"<p>The percentage of participants who shouldn't continue the journey.</p>\
  \ <p>To determine which participants are held out, Amazon Pinpoint applies a probability-based algorithm to the percentage that you specify. Therefore, the actual percentage of participants who are held out may not be equal to the percentage that you specify.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Percentage\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-holdout-activity-schema.json
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
title: HoldoutActivity
---
