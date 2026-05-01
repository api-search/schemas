---
description: Specifies a segment to associate with an activity in a journey.
layout: schema
name: SegmentCondition
properties_list:
- description: ''
  name: SegmentId
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-segment-condition-schema.json
slug: amazon-pinpoint-segment-condition
source_filename: amazon-pinpoint-segment-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-condition-schema.json\",\n  \"title\": \"SegmentCondition\",\n  \"description\": \"Specifies a segment to associate with an activity in a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SegmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the segment to associate with the activity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SegmentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-condition-schema.json
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
title: SegmentCondition
---
