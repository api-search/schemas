---
description: A DMI station feature describing a meteorological or oceanographic measurement station.
layout: schema
name: Station
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
schema_file: json-schema/station.json
slug: station
source_filename: station.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/danish-meteorological-institutes/refs/heads/main/json-schema/station.json\",\n  \"title\": \"Station\",\n  \"description\": \"A DMI station feature describing a meteorological or oceanographic measurement station.\",\n  \"type\": \"object\",\n  \"required\": [\"type\", \"geometry\", \"properties\"],\n  \"properties\": {\n    \"type\": {\"type\": \"string\", \"const\": \"Feature\"},\n    \"id\": {\"type\": \"string\"},\n    \"geometry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\"type\": \"string\"},\n        \"coordinates\": {\"type\": \"array\"}\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"stationId\": {\"type\": \"string\"},\n        \"name\": {\"type\": \"string\"},\n        \"country\": {\"type\": \"string\"},\n        \"type\": {\"type\": \"string\"\
  },\n        \"operationFrom\": {\"type\": \"string\", \"format\": \"date-time\"},\n        \"operationTo\": {\"type\": \"string\", \"format\": \"date-time\"}\n      },\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/danish-meteorological-institutes/refs/heads/main/json-schema/station.json
tags:
- Climate
- Environment
- Lightning
- Meteorological
- Ocean
- Open Data
- Weather
title: Station
---
