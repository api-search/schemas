---
description: ''
layout: schema
name: FlightStatusForecastResponse
properties_list:
- description: ''
  name: timestamp
  type: string
- description: ''
  name: uav_model
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: weather_source
  type: string
- description: ''
  name: location
  type: object
- description: ''
  name: weather_params
  type: object
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-weather-service-flightstatusforecastresponse-schema.json
slug: agstack-openagri-weather-service-flightstatusforecastresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/FlightStatusForecastResponse.json\",\n  \"title\": \"FlightStatusForecastResponse\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Timestamp\"\n    },\n    \"uav_model\": {\n      \"type\": \"string\",\n      \"title\": \"Uav Model\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"title\": \"Status\"\n    },\n    \"weather_source\": {\n      \"type\": \"string\",\n      \"title\": \"Weather Source\"\n    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/GeoJSONOut\"\n    },\n    \"weather_params\": {\n      \"additionalProperties\": {\n        \"type\": \"number\"\n      },\n      \"type\": \"object\",\n      \"title\": \"Weather Params\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"timestamp\",\n    \"uav_model\",\n    \"status\",\n    \"\
  weather_source\",\n    \"location\",\n    \"weather_params\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-weather-service-flightstatusforecastresponse-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: FlightStatusForecastResponse
---
