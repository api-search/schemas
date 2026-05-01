---
description: Provides information about a session.
layout: schema
name: Session
properties_list:
- description: ''
  name: Duration
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: StartTimestamp
  type: object
- description: ''
  name: StopTimestamp
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-session-schema.json
slug: amazon-pinpoint-session
source_filename: amazon-pinpoint-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-session-schema.json\",\n  \"title\": \"Session\",\n  \"description\": \"Provides information about a session.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The duration of the session, in milliseconds.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the session.\"\n        }\n      ]\n    },\n    \"StartTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and\
  \ time when the session began.\"\n        }\n      ]\n    },\n    \"StopTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time when the session ended.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"StartTimestamp\",\n    \"Id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-session-schema.json
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
title: Session
---
