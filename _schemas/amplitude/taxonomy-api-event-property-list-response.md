---
description: EventPropertyListResponse schema from Amplitude Taxonomy API
layout: schema
name: EventPropertyListResponse
properties_list:
- description: Array of event properties.
  name: data
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/taxonomy-api-event-property-list-response-schema.json
slug: taxonomy-api-event-property-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-event-property-list-response-schema.json\",\n  \"title\": \"EventPropertyListResponse\",\n  \"description\": \"EventPropertyListResponse schema from Amplitude Taxonomy API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of event properties.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"event_property\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the event property.\"\n          },\n          \"event_type\": {\n            \"type\": \"string\",\n            \"description\": \"The event type this property belongs to.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A description\
  \ of the event property.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The data type of the property.\"\n          },\n          \"is_required\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the property is required.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-event-property-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: EventPropertyListResponse
---
