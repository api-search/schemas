---
description: ''
layout: schema
name: PredictionOut
properties_list:
- description: ''
  name: value
  type: number
- description: ''
  name: timestamp
  type: string
- description: ''
  name: source
  type: string
- description: ''
  name: spatial_entity
  type: object
- description: ''
  name: data_type
  type: string
- description: ''
  name: measurement_type
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-weather-service-predictionout-schema.json
slug: agstack-openagri-weather-service-predictionout
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/PredictionOut.json\",\n  \"title\": \"PredictionOut\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"number\",\n      \"title\": \"Value\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Timestamp\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"title\": \"Source\"\n    },\n    \"spatial_entity\": {\n      \"$ref\": \"#/components/schemas/PointOut\"\n    },\n    \"data_type\": {\n      \"type\": \"string\",\n      \"title\": \"Data Type\"\n    },\n    \"measurement_type\": {\n      \"type\": \"string\",\n      \"title\": \"Measurement Type\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"value\",\n    \"timestamp\",\n    \"source\",\n    \"spatial_entity\",\n    \"data_type\",\n    \"measurement_type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-weather-service-predictionout-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: PredictionOut
---
