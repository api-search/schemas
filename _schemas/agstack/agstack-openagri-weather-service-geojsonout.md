---
description: ''
layout: schema
name: GeoJSONOut
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: coordinates
  type: array
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-weather-service-geojsonout-schema.json
slug: agstack-openagri-weather-service-geojsonout
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/GeoJSONOut.json\",\n  \"title\": \"GeoJSONOut\",\n  \"properties\": {\n    \"type\": {\n      \"$ref\": \"#/components/schemas/GeoJSONTypeEnum\"\n    },\n    \"coordinates\": {\n      \"items\": {},\n      \"type\": \"array\",\n      \"title\": \"Coordinates\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"type\",\n    \"coordinates\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-weather-service-geojsonout-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: GeoJSONOut
---
