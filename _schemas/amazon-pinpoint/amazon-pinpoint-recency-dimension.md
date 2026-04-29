---
description: Specifies criteria for including or excluding endpoints from a segment based on how recently an endpoint was active.
layout: schema
name: RecencyDimension
properties_list:
- description: ''
  name: Duration
  type: object
- description: ''
  name: RecencyType
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-recency-dimension-schema.json
slug: amazon-pinpoint-recency-dimension
source_filename: amazon-pinpoint-recency-dimension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-recency-dimension-schema.json\",\n  \"title\": \"RecencyDimension\",\n  \"description\": \"Specifies criteria for including or excluding endpoints from a segment based on how recently an endpoint was active.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"The duration to use when determining whether an endpoint is active or inactive.\"\n        }\n      ]\n    },\n    \"RecencyType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecencyType\"\n        },\n        {\n          \"description\": \"The type of recency dimension to use for the segment. Valid values are: ACTIVE, endpoints that were active\
  \ within the specified duration are included in the segment; and, INACTIVE, endpoints that weren't active within the specified duration are included in the segment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Duration\",\n    \"RecencyType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-recency-dimension-schema.json
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
title: RecencyDimension
---
