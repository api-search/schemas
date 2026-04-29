---
description: ''
layout: schema
name: GeojsonGeometry
properties_list:
- description: A valid geojson geometry coordinates
  name: geometry
  type: object
- description: ''
  name: type
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-geojson-geometry-schema.json
slug: oneatlas-geojson-geometry
source_filename: oneatlas-geojson-geometry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-geojson-geometry-schema.json\",\n  \"title\": \"GeojsonGeometry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"geometry\": {\n      \"description\": \"A valid geojson geometry coordinates\",\n      \"type\": \"object\"\n    },\n    \"type\": {\n      \"enum\": [\n        \"Polygon\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-geojson-geometry-schema.json
tags:
- Imagery
- Satellites
title: GeojsonGeometry
---
