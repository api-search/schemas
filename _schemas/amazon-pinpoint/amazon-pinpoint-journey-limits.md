---
description: Specifies limits on the messages that a journey can send and the number of times participants can enter a journey.
layout: schema
name: JourneyLimits
properties_list:
- description: ''
  name: DailyCap
  type: object
- description: ''
  name: EndpointReentryCap
  type: object
- description: ''
  name: MessagesPerSecond
  type: object
- description: ''
  name: EndpointReentryInterval
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-journey-limits-schema.json
slug: amazon-pinpoint-journey-limits
source_filename: amazon-pinpoint-journey-limits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-limits-schema.json\",\n  \"title\": \"JourneyLimits\",\n  \"description\": \"Specifies limits on the messages that a journey can send and the number of times participants can enter a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DailyCap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of messages that the journey can send to a single participant during a 24-hour period. The maximum value is 100.\"\n        }\n      ]\n    },\n    \"EndpointReentryCap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of times that a participant can enter\
  \ the journey. The maximum value is 100. To allow participants to enter the journey an unlimited number of times, set this value to 0.\"\n        }\n      ]\n    },\n    \"MessagesPerSecond\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of messages that the journey can send each second.\"\n        }\n      ]\n    },\n    \"EndpointReentryInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Minimum time that must pass before an endpoint can re-enter a given journey. The duration should use an ISO 8601 format, such as PT1H. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-limits-schema.json
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
title: JourneyLimits
---
