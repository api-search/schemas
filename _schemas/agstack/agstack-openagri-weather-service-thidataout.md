---
description: ''
layout: schema
name: THIDataOut
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: spatial_entity
  type: object
- description: ''
  name: thi
  type: number
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-weather-service-thidataout-schema.json
slug: agstack-openagri-weather-service-thidataout
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/THIDataOut.json\",\n  \"title\": \"THIDataOut\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"title\": \"Id\"\n    },\n    \"spatial_entity\": {\n      \"$ref\": \"#/components/schemas/PointOut\"\n    },\n    \"thi\": {\n      \"type\": \"number\",\n      \"title\": \"Thi\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"spatial_entity\",\n    \"thi\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-weather-service-thidataout-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: THIDataOut
---
