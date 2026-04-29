---
description: Specifies the settings for an event that causes a campaign to be sent or a journey activity to be performed.
layout: schema
name: EventFilter
properties_list:
- description: ''
  name: Dimensions
  type: object
- description: ''
  name: FilterType
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-event-filter-schema.json
slug: amazon-pinpoint-event-filter
source_filename: amazon-pinpoint-event-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-filter-schema.json\",\n  \"title\": \"EventFilter\",\n  \"description\": \"Specifies the settings for an event that causes a campaign to be sent or a journey activity to be performed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Dimensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventDimensions\"\n        },\n        {\n          \"description\": \"The dimensions for the event filter to use for the campaign or the journey activity.\"\n        }\n      ]\n    },\n    \"FilterType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterType\"\n        },\n        {\n          \"description\": \"The type of event that causes the campaign to be sent or the journey activity to be performed. Valid values are:\
  \ SYSTEM, sends the campaign or performs the activity when a system event occurs; and, ENDPOINT, sends the campaign or performs the activity when an endpoint event (<link  linkend=\\\"apps-application-id-events\\\">Events resource</link>) occurs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FilterType\",\n    \"Dimensions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-filter-schema.json
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
title: EventFilter
---
