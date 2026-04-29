---
description: Specifies a condition to evaluate for an activity path in a journey.
layout: schema
name: MultiConditionalBranch
properties_list:
- description: ''
  name: Condition
  type: object
- description: ''
  name: NextActivity
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-multi-conditional-branch-schema.json
slug: amazon-pinpoint-multi-conditional-branch
source_filename: amazon-pinpoint-multi-conditional-branch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-multi-conditional-branch-schema.json\",\n  \"title\": \"MultiConditionalBranch\",\n  \"description\": \"Specifies a condition to evaluate for an activity path in a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Condition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimpleCondition\"\n        },\n        {\n          \"description\": \"The condition to evaluate for the activity path.\"\n        }\n      ]\n    },\n    \"NextActivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the next activity to perform, after completing the activity for the path.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-multi-conditional-branch-schema.json
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
title: MultiConditionalBranch
---
