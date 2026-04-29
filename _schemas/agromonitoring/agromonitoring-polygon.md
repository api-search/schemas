---
description: A registered field polygon for crop monitoring.
layout: schema
name: Polygon
properties_list:
- description: Unique identifier for the polygon.
  name: id
  type: string
- description: Display name for the polygon/field.
  name: name
  type: string
- description: Field area in hectares.
  name: area
  type: number
- description: Timestamp when the polygon was created.
  name: created_at
  type: string
- description: ''
  name: geo_json
  type: object
provider_name: Agromonitoring
provider_slug: agromonitoring
schema_file: json-schema/agromonitoring-polygon-schema.json
slug: agromonitoring-polygon
source_filename: agromonitoring-polygon-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.agromonitoring.com/schemas/Polygon.json\",\n  \"title\": \"Polygon\",\n  \"type\": \"object\",\n  \"description\": \"A registered field polygon for crop monitoring.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the polygon.\",\n      \"example\": \"poly-500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the polygon/field.\",\n      \"example\": \"North Field\"\n    },\n    \"area\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Field area in hectares.\",\n      \"example\": 45.2\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the polygon was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"geo_json\": {\n    \
  \  \"$ref\": \"#/components/schemas/GeoJson\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/json-schema/agromonitoring-polygon-schema.json
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
title: Polygon
---
