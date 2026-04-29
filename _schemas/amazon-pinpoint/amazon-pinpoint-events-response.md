---
description: Provides information about endpoints and the events that they're associated with.
layout: schema
name: EventsResponse
properties_list:
- description: ''
  name: Results
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-events-response-schema.json
slug: amazon-pinpoint-events-response
source_filename: amazon-pinpoint-events-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-events-response-schema.json\",\n  \"title\": \"EventsResponse\",\n  \"description\": \"Provides information about endpoints and the events that they're associated with.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Results\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfItemResponse\"\n        },\n        {\n          \"description\": \"A map that contains a multipart response for each endpoint. For each item in this object, the endpoint ID is the key and the item response is the value. If no item response exists, the value can also be one of the following: 202, the request was processed successfully; or 400, the payload wasn't valid or required fields were missing.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-events-response-schema.json
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
title: EventsResponse
---
