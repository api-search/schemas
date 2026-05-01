---
description: A single weather, climate, ocean, or lightning observation returned by the DMI Open Data API as a GeoJSON Feature.
layout: schema
name: Observation
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: geometry
  type: object
- description: ''
  name: properties
  type: object
provider_name: Danish Meteorological Institutes
provider_slug: danish-meteorological-institutes
schema_file: json-schema/observation.json
slug: observation
source_filename: observation.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/danish-meteorological-institutes/refs/heads/main/json-schema/observation.json\",\n  \"title\": \"Observation\",\n  \"description\": \"A single weather, climate, ocean, or lightning observation returned by the DMI Open Data API as a GeoJSON Feature.\",\n  \"type\": \"object\",\n  \"required\": [\"type\", \"geometry\", \"properties\"],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"Feature\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"geometry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\"type\": \"string\"},\n        \"coordinates\": {\"type\": \"array\"}\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"stationId\": {\"type\": \"string\"},\n        \"parameterId\": {\"type\": \"string\"},\n     \
  \   \"observed\": {\"type\": \"string\", \"format\": \"date-time\"},\n        \"value\": {\"type\": \"number\"}\n      },\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/danish-meteorological-institutes/refs/heads/main/json-schema/observation.json
tags:
- Climate
- Environment
- Lightning
- Meteorological
- Ocean
- Open Data
- Weather
title: Observation
---
