---
description: EventProperty schema from Amplitude Taxonomy API
layout: schema
name: EventProperty
properties_list:
- description: The name of the event property.
  name: event_property
  type: string
- description: The event type this property belongs to.
  name: event_type
  type: string
- description: A description of the event property.
  name: description
  type: string
- description: The data type of the property.
  name: type
  type: string
- description: Whether the property is required.
  name: is_required
  type: boolean
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/taxonomy-api-event-property-schema.json
slug: taxonomy-api-event-property
source_filename: taxonomy-api-event-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-event-property-schema.json\",\n  \"title\": \"EventProperty\",\n  \"description\": \"EventProperty schema from Amplitude Taxonomy API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"event_property\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the event property.\"\n    },\n    \"event_type\": {\n      \"type\": \"string\",\n      \"description\": \"The event type this property belongs to.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the event property.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the property.\"\n    },\n    \"is_required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the property is required.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-event-property-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: EventProperty
---
