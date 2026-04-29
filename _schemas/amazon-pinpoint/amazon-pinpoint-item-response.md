---
description: Provides information about the results of a request to create or update an endpoint that's associated with an event.
layout: schema
name: ItemResponse
properties_list:
- description: ''
  name: EndpointItemResponse
  type: object
- description: ''
  name: EventsItemResponse
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-item-response-schema.json
slug: amazon-pinpoint-item-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-item-response-schema.json\",\n  \"title\": \"ItemResponse\",\n  \"description\": \"Provides information about the results of a request to create or update an endpoint that's associated with an event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointItemResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointItemResponse\"\n        },\n        {\n          \"description\": \"The response that was received after the endpoint data was accepted.\"\n        }\n      ]\n    },\n    \"EventsItemResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfEventItemResponse\"\n        },\n        {\n          \"description\": \"A multipart response object that contains a key and a value for each event in the\
  \ request. In each object, the event ID is the key and an EventItemResponse object is the value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-item-response-schema.json
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
title: ItemResponse
---
