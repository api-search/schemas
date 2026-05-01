---
description: Specifies the settings for a random split activity in a journey. This type of activity randomly sends specified percentages of participants down one of as many as five paths in a journey, based on conditions that you specify.
layout: schema
name: RandomSplitActivity
properties_list:
- description: ''
  name: Branches
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-random-split-activity-schema.json
slug: amazon-pinpoint-random-split-activity
source_filename: amazon-pinpoint-random-split-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-random-split-activity-schema.json\",\n  \"title\": \"RandomSplitActivity\",\n  \"description\": \"Specifies the settings for a random split activity in a journey. This type of activity randomly sends specified percentages of participants down one of as many as five paths in a journey, based on conditions that you specify.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Branches\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfRandomSplitEntry\"\n        },\n        {\n          \"description\": \"The paths for the activity, including the percentage of participants to enter each path and the activity to perform for each path.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-random-split-activity-schema.json
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
title: RandomSplitActivity
---
