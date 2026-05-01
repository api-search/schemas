---
description: Specifies a batch of endpoints and events to process.
layout: schema
name: EventsBatch
properties_list:
- description: ''
  name: Endpoint
  type: object
- description: ''
  name: Events
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-events-batch-schema.json
slug: amazon-pinpoint-events-batch
source_filename: amazon-pinpoint-events-batch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-events-batch-schema.json\",\n  \"title\": \"EventsBatch\",\n  \"description\": \"Specifies a batch of endpoints and events to process.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Endpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublicEndpoint\"\n        },\n        {\n          \"description\": \"A set of properties and attributes that are associated with the endpoint.\"\n        }\n      ]\n    },\n    \"Events\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfEvent\"\n        },\n        {\n          \"description\": \"A set of properties that are associated with the event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Endpoint\",\n    \"Events\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-events-batch-schema.json
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
title: EventsBatch
---
