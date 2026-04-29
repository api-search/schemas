---
description: ''
layout: schema
name: PointOut
properties_list:
- description: ''
  name: location
  type: object
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-weather-service-pointout-schema.json
slug: agstack-openagri-weather-service-pointout
source_filename: agstack-openagri-weather-service-pointout-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/PointOut.json\",\n  \"title\": \"PointOut\",\n  \"properties\": {\n    \"location\": {\n      \"$ref\": \"#/components/schemas/GeoJSONOut\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-weather-service-pointout-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: PointOut
---
