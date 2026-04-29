---
description: Specifies a condition to evaluate for an activity in a journey.
layout: schema
name: SimpleCondition
properties_list:
- description: ''
  name: EventCondition
  type: object
- description: ''
  name: SegmentCondition
  type: object
- description: ''
  name: SegmentDimensions
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-simple-condition-schema.json
slug: amazon-pinpoint-simple-condition
source_filename: amazon-pinpoint-simple-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-simple-condition-schema.json\",\n  \"title\": \"SimpleCondition\",\n  \"description\": \"Specifies a condition to evaluate for an activity in a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventCondition\"\n        },\n        {\n          \"description\": \"The dimension settings for the event that's associated with the activity.\"\n        }\n      ]\n    },\n    \"SegmentCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentCondition\"\n        },\n        {\n          \"description\": \"The segment that's associated with the activity.\"\n        }\n      ]\n    },\n    \"SegmentDimensions\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/SegmentDimensions\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentDimensions\"\n          },\n          \"description\": \"The dimension settings for the segment that's associated with the activity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-simple-condition-schema.json
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
title: SimpleCondition
---
