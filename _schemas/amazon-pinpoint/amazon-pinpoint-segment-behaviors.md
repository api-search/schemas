---
description: Specifies dimension settings for including or excluding endpoints from a segment based on how recently an endpoint was active.
layout: schema
name: SegmentBehaviors
properties_list:
- description: ''
  name: Recency
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-segment-behaviors-schema.json
slug: amazon-pinpoint-segment-behaviors
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-behaviors-schema.json\",\n  \"title\": \"SegmentBehaviors\",\n  \"description\": \"Specifies dimension settings for including or excluding endpoints from a segment based on how recently an endpoint was active.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Recency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecencyDimension\"\n        },\n        {\n          \"description\": \"The dimension settings that are based on how recently an endpoint was active.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-behaviors-schema.json
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
title: SegmentBehaviors
---
