---
description: Specifies a batch of events to process.
layout: schema
name: EventsRequest
properties_list:
- description: ''
  name: BatchItem
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-events-request-schema.json
slug: amazon-pinpoint-events-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-events-request-schema.json\",\n  \"title\": \"EventsRequest\",\n  \"description\": \"Specifies a batch of events to process.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BatchItem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfEventsBatch\"\n        },\n        {\n          \"description\": \"The batch of events to process. For each item in a batch, the endpoint ID acts as a key that has an EventsBatch object as its value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BatchItem\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-events-request-schema.json
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
title: EventsRequest
---
