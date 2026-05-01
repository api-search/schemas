---
description: Specifies the settings for an event that causes a journey activity to start.
layout: schema
name: EventStartCondition
properties_list:
- description: ''
  name: EventFilter
  type: object
- description: ''
  name: SegmentId
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-event-start-condition-schema.json
slug: amazon-pinpoint-event-start-condition
source_filename: amazon-pinpoint-event-start-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-start-condition-schema.json\",\n  \"title\": \"EventStartCondition\",\n  \"description\": \"Specifies the settings for an event that causes a journey activity to start.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventFilter\": {\n      \"$ref\": \"#/components/schemas/EventFilter\"\n    },\n    \"SegmentId\": {\n      \"$ref\": \"#/components/schemas/__string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-start-condition-schema.json
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
title: EventStartCondition
---
