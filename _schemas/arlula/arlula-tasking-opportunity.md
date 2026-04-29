---
description: A future satellite capture opportunity.
layout: schema
name: TaskingOpportunity
properties_list:
- description: Ordering ID for this tasking opportunity.
  name: id
  type: string
- description: Supplier identifier.
  name: supplier
  type: string
- description: Earliest start time for the capture window.
  name: captureStart
  type: string
- description: Latest end time for the capture window.
  name: captureEnd
  type: string
- description: Expected ground sample distance in meters.
  name: gsd
  type: number
- description: Price for this tasking opportunity.
  name: price
  type: number
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-tasking-opportunity-schema.json
slug: arlula-tasking-opportunity
source_filename: arlula-tasking-opportunity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/tasking-opportunity.json\",\n  \"title\": \"TaskingOpportunity\",\n  \"description\": \"A future satellite capture opportunity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Ordering ID for this tasking opportunity.\",\n      \"examples\": [\n        \"opp-a1b2c3d4\"\n      ]\n    },\n    \"supplier\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier identifier.\",\n      \"examples\": [\n        \"supplier-001\"\n      ]\n    },\n    \"captureStart\": {\n      \"type\": \"string\",\n      \"description\": \"Earliest start time for the capture window.\",\n      \"examples\": [\n        \"2026-05-10T10:00:00Z\"\n      ]\n    },\n    \"captureEnd\": {\n      \"type\": \"string\",\n      \"description\": \"Latest end time for the capture window.\",\n      \"examples\": [\n    \
  \    \"2026-05-10T10:05:00Z\"\n      ]\n    },\n    \"gsd\": {\n      \"type\": \"number\",\n      \"description\": \"Expected ground sample distance in meters.\",\n      \"examples\": [\n        0.5\n      ]\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Price for this tasking opportunity.\",\n      \"examples\": [\n        500.0\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-tasking-opportunity-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: TaskingOpportunity
---
