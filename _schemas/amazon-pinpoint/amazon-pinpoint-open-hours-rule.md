---
description: List of OpenHours Rules.
layout: schema
name: OpenHoursRule
properties_list:
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-open-hours-rule-schema.json
slug: amazon-pinpoint-open-hours-rule
source_filename: amazon-pinpoint-open-hours-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-open-hours-rule-schema.json\",\n  \"title\": \"OpenHoursRule\",\n  \"description\": \"List of OpenHours Rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Local start time in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Local start time in ISO 8601 format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-open-hours-rule-schema.json
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
title: OpenHoursRule
---
