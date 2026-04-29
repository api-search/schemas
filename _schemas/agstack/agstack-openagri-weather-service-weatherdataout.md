---
description: ''
layout: schema
name: WeatherDataOut
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: spatial_entity
  type: object
- description: ''
  name: data
  type: object
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-weather-service-weatherdataout-schema.json
slug: agstack-openagri-weather-service-weatherdataout
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/WeatherDataOut.json\",\n  \"title\": \"WeatherDataOut\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"title\": \"Id\"\n    },\n    \"spatial_entity\": {\n      \"$ref\": \"#/components/schemas/PointOut\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"title\": \"Data\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"spatial_entity\",\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-weather-service-weatherdataout-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: WeatherDataOut
---
