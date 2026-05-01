---
description: Specifies the settings for a path in a random split activity in a journey.
layout: schema
name: RandomSplitEntry
properties_list:
- description: ''
  name: NextActivity
  type: object
- description: ''
  name: Percentage
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-random-split-entry-schema.json
slug: amazon-pinpoint-random-split-entry
source_filename: amazon-pinpoint-random-split-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-random-split-entry-schema.json\",\n  \"title\": \"RandomSplitEntry\",\n  \"description\": \"Specifies the settings for a path in a random split activity in a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextActivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the next activity to perform, after completing the activity for the path.\"\n        }\n      ]\n    },\n    \"Percentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"<p>The percentage of participants to send down the activity path.</p> <p>To determine which participants are sent down each\
  \ path, Amazon Pinpoint applies a probability-based algorithm to the percentages that you specify for the paths. Therefore, the actual percentage of participants who are sent down a path may not be equal to the percentage that you specify.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-random-split-entry-schema.json
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
title: RandomSplitEntry
---
