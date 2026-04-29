---
description: A Cribl route that applies filter expressions on incoming data events to direct matching results to the appropriate pipeline and destination for processing and delivery.
layout: schema
name: Cribl Route
properties_list:
- description: Unique identifier for the route
  name: id
  type: string
- description: Human-readable display name for the route
  name: name
  type: string
- description: JavaScript filter expression that determines which events match this route. Use true to match all events.
  name: filter
  type: string
- description: The pipeline identifier to process matching events through
  name: pipeline
  type: string
- description: The destination identifier where processed events are sent
  name: output
  type: string
- description: Whether matching events stop being evaluated by subsequent routes in the route table
  name: final
  type: boolean
- description: Whether this route is disabled and should be skipped during evaluation
  name: disabled
  type: boolean
- description: A human-readable description of the route purpose and behavior
  name: description
  type: string
- description: Worker group or fleet-specific route configuration overrides
  name: groups
  type: object
- description: Additional pipeline and destination pairs that receive copies of matching events
  name: clones
  type: array
provider_name: Cribl
provider_slug: cribl
schema_file: json-schema/cribl-route-schema.json
slug: cribl-route
source_filename: cribl-route-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.cribl.io/schemas/cribl/route.json\",\n  \"title\": \"Cribl Route\",\n  \"description\": \"A Cribl route that applies filter expressions on incoming data events to direct matching results to the appropriate pipeline and destination for processing and delivery.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"filter\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the route\",\n      \"pattern\": \"^[a-zA-Z0-9_-]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the route\"\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"JavaScript filter expression that determines which events match this route. Use true to match all events.\"\n    },\n    \"pipeline\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"The pipeline identifier to process matching events through\"\n    },\n    \"output\": {\n      \"type\": \"string\",\n      \"description\": \"The destination identifier where processed events are sent\"\n    },\n    \"final\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether matching events stop being evaluated by subsequent routes in the route table\",\n      \"default\": true\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this route is disabled and should be skipped during evaluation\",\n      \"default\": false\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the route purpose and behavior\"\n    },\n    \"groups\": {\n      \"type\": \"object\",\n      \"description\": \"Worker group or fleet-specific route configuration overrides\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"description\": \"Group-specific route\
  \ settings\"\n      }\n    },\n    \"clones\": {\n      \"type\": \"array\",\n      \"description\": \"Additional pipeline and destination pairs that receive copies of matching events\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RouteClone\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"RouteClone\": {\n      \"type\": \"object\",\n      \"description\": \"A clone destination that receives a copy of events matching the parent route.\",\n      \"properties\": {\n        \"pipeline\": {\n          \"type\": \"string\",\n          \"description\": \"The pipeline identifier for processing cloned events\"\n        },\n        \"output\": {\n          \"type\": \"string\",\n          \"description\": \"The destination identifier for the cloned events\"\n        },\n        \"filter\": {\n          \"type\": \"string\",\n          \"description\": \"Additional filter expression for this clone\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/json-schema/cribl-route-schema.json
tags:
- Configuration
- Data Lake
- Data Pipelines
- Data Routing
- Edge Computing
- Infrastructure as Code
- Observability
- Search
- Security Data
- Stream Processing
- Telemetry
title: Cribl Route
---
