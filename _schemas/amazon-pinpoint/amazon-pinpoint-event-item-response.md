---
description: Provides the status code and message that result from processing an event.
layout: schema
name: EventItemResponse
properties_list:
- description: ''
  name: Message
  type: object
- description: ''
  name: StatusCode
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-event-item-response-schema.json
slug: amazon-pinpoint-event-item-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-item-response-schema.json\",\n  \"title\": \"EventItemResponse\",\n  \"description\": \"Provides the status code and message that result from processing an event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A custom message that's returned in the response as a result of processing the event.\"\n        }\n      ]\n    },\n    \"StatusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The status code that's returned in the response as a result of processing the event. Possible values are: 202, for events that were accepted;\
  \ and, 400, for events that weren't valid.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-item-response-schema.json
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
title: EventItemResponse
---
