---
description: Specifies the dimensions for an event filter that determines when a campaign is sent or a journey activity is performed.
layout: schema
name: EventDimensions
properties_list:
- description: ''
  name: Attributes
  type: object
- description: ''
  name: EventType
  type: object
- description: ''
  name: Metrics
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-event-dimensions-schema.json
slug: amazon-pinpoint-event-dimensions
source_filename: amazon-pinpoint-event-dimensions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-dimensions-schema.json\",\n  \"title\": \"EventDimensions\",\n  \"description\": \"Specifies the dimensions for an event filter that determines when a campaign is sent or a journey activity is performed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfAttributeDimension\"\n        },\n        {\n          \"description\": \"One or more custom attributes that your application reports to Amazon Pinpoint. You can use these attributes as selection criteria when you create an event filter.\"\n        }\n      ]\n    },\n    \"EventType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetDimension\"\n        },\n        {\n          \"description\": \"The\
  \ name of the event that causes the campaign to be sent or the journey activity to be performed. This can be a standard event that Amazon Pinpoint generates, such as _email.delivered. For campaigns, this can also be a custom event that's specific to your application. For information about standard events, see <a href=\\\"https://docs.aws.amazon.com/pinpoint/latest/developerguide/event-streams.html\\\">Streaming Amazon Pinpoint Events</a> in the <i>Amazon Pinpoint Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfMetricDimension\"\n        },\n        {\n          \"description\": \"One or more custom metrics that your application reports to Amazon Pinpoint. You can use these metrics as selection criteria when you create an event filter.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-dimensions-schema.json
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
title: EventDimensions
---
