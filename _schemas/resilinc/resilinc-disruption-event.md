---
description: JSON Schema for a Resilinc supply chain disruption event, representing a real-world event (natural disaster, geopolitical, factory fire, etc.) that may impact supply chain operations.
layout: schema
name: Resilinc Disruption Event
properties_list:
- description: Unique event identifier.
  name: id
  type: string
- description: Event title or headline.
  name: title
  type: string
- description: Detailed description of the disruption event.
  name: description
  type: string
- description: Category of the disruption event.
  name: event_type
  type: string
- description: Severity level of the event.
  name: severity
  type: string
- description: Current status of the event.
  name: status
  type: string
- description: Geographic location of the event.
  name: location
  type: object
- description: Suppliers potentially impacted by this event.
  name: affected_suppliers
  type: array
- description: Parts or components potentially impacted.
  name: affected_parts
  type: array
- description: Timestamp when the event was published.
  name: published_at
  type: string
- description: Timestamp when the event started.
  name: started_at
  type: string
- description: Timestamp when the event was resolved (null if ongoing).
  name: resolved_at
  type:
  - string
  - 'null'
- description: External source URLs for the event.
  name: source_urls
  type: array
provider_name: Resilinc
provider_slug: resilinc
schema_file: json-schema/resilinc-disruption-event-schema.json
slug: resilinc-disruption-event
source_filename: resilinc-disruption-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/resilinc/json-schema/resilinc-disruption-event-schema.json\",\n  \"title\": \"Resilinc Disruption Event\",\n  \"description\": \"JSON Schema for a Resilinc supply chain disruption event, representing a real-world event (natural disaster, geopolitical, factory fire, etc.) that may impact supply chain operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique event identifier.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Event title or headline.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the disruption event.\"\n    },\n    \"event_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"natural_disaster\",\n        \"geopolitical\",\n        \"factory_fire\",\n    \
  \    \"labor_strike\",\n        \"port_disruption\",\n        \"logistics\",\n        \"cyber_attack\",\n        \"regulatory\",\n        \"pandemic\",\n        \"financial\",\n        \"other\"\n      ],\n      \"description\": \"Category of the disruption event.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\"low\", \"medium\", \"high\", \"critical\"],\n      \"description\": \"Severity level of the event.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"monitoring\", \"resolved\"],\n      \"description\": \"Current status of the event.\"\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"Geographic location of the event.\",\n      \"properties\": {\n        \"country\": { \"type\": \"string\" },\n        \"region\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"lat\": { \"type\": \"number\" },\n        \"lon\": { \"type\": \"number\" }\n     \
  \ }\n    },\n    \"affected_suppliers\": {\n      \"type\": \"array\",\n      \"description\": \"Suppliers potentially impacted by this event.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"supplier_id\": { \"type\": \"string\" },\n          \"supplier_name\": { \"type\": \"string\" },\n          \"impact_level\": {\n            \"type\": \"string\",\n            \"enum\": [\"low\", \"medium\", \"high\", \"critical\"]\n          }\n        }\n      }\n    },\n    \"affected_parts\": {\n      \"type\": \"array\",\n      \"description\": \"Parts or components potentially impacted.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"part_id\": { \"type\": \"string\" },\n          \"part_number\": { \"type\": \"string\" },\n          \"description\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"published_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Timestamp when the event was published.\"\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the event started.\"\n    },\n    \"resolved_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the event was resolved (null if ongoing).\"\n    },\n    \"source_urls\": {\n      \"type\": \"array\",\n      \"description\": \"External source URLs for the event.\",\n      \"items\": { \"type\": \"string\", \"format\": \"uri\" }\n    }\n  },\n  \"required\": [\"id\", \"title\", \"event_type\", \"severity\", \"status\", \"published_at\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/resilinc/refs/heads/main/json-schema/resilinc-disruption-event-schema.json
tags:
- Supply Chain
- Risk Management
- Supplier Intelligence
- Disruption Monitoring
- AI
title: Resilinc Disruption Event
---
