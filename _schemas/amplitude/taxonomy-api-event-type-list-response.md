---
description: EventTypeListResponse schema from Amplitude Taxonomy API
layout: schema
name: EventTypeListResponse
properties_list:
- description: Array of event types.
  name: data
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/taxonomy-api-event-type-list-response-schema.json
slug: taxonomy-api-event-type-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-event-type-list-response-schema.json\",\n  \"title\": \"EventTypeListResponse\",\n  \"description\": \"EventTypeListResponse schema from Amplitude Taxonomy API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of event types.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"event_type\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the event type.\"\n          },\n          \"category\": {\n            \"$ref\": \"#/components/schemas/Category\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A description of the event type.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-event-type-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: EventTypeListResponse
---
