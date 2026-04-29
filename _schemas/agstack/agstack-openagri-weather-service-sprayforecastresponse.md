---
description: ''
layout: schema
name: SprayForecastResponse
properties_list:
- description: ''
  name: timestamp
  type: string
- description: ''
  name: spray_conditions
  type: object
- description: ''
  name: source
  type: string
- description: ''
  name: location
  type: object
- description: ''
  name: detailed_status
  type: object
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-weather-service-sprayforecastresponse-schema.json
slug: agstack-openagri-weather-service-sprayforecastresponse
source_filename: agstack-openagri-weather-service-sprayforecastresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/SprayForecastResponse.json\",\n  \"title\": \"SprayForecastResponse\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Timestamp\"\n    },\n    \"spray_conditions\": {\n      \"$ref\": \"#/components/schemas/SprayStatus\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"title\": \"Source\"\n    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/GeoJSONOut\"\n    },\n    \"detailed_status\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"object\",\n      \"title\": \"Detailed Status\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"timestamp\",\n    \"spray_conditions\",\n    \"source\",\n    \"location\",\n    \"detailed_status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-weather-service-sprayforecastresponse-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: SprayForecastResponse
---
