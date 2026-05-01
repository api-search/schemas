---
description: Closed Days Rule. Part of Journey sending schedule.
layout: schema
name: ClosedDaysRule
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: StartDateTime
  type: object
- description: ''
  name: EndDateTime
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-closed-days-rule-schema.json
slug: amazon-pinpoint-closed-days-rule
source_filename: amazon-pinpoint-closed-days-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-closed-days-rule-schema.json\",\n  \"title\": \"ClosedDaysRule\",\n  \"description\": \"Closed Days Rule. Part of Journey sending schedule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Name of the rule.\"\n        }\n      ]\n    },\n    \"StartDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Start Datetime in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"EndDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"End Datetime\
  \ in ISO 8601 format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-closed-days-rule-schema.json
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
title: ClosedDaysRule
---
