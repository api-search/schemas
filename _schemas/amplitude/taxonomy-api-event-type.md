---
description: EventType schema from Amplitude Taxonomy API
layout: schema
name: EventType
properties_list:
- description: The name of the event type.
  name: event_type
  type: string
- description: ''
  name: category
  type: object
- description: A description of the event type.
  name: description
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/taxonomy-api-event-type-schema.json
slug: taxonomy-api-event-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-event-type-schema.json\",\n  \"title\": \"EventType\",\n  \"description\": \"EventType schema from Amplitude Taxonomy API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"event_type\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the event type.\"\n    },\n    \"category\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique identifier of the category.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the category.\"\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the event type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-event-type-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: EventType
---
