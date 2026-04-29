---
description: Air quality monitoring station with current readings
layout: schema
name: AQIStation
properties_list:
- description: Response status (ok or error)
  name: status
  type: string
- description: ''
  name: data
  type: object
provider_name: Air Quality Programmatic APIs
provider_slug: air-quality-programmatic-apis
schema_file: json-schema/aqicn-aqi-station-schema.json
slug: aqicn-aqi-station
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-aqi-station-schema.json\",\n  \"title\": \"AQIStation\",\n  \"description\": \"Air quality monitoring station with current readings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Response status (ok or error)\",\n      \"example\": \"ok\"\n    },\n    \"data\": {\n      \"$ref\": \"#/components/schemas/StationData\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-aqi-station-schema.json
tags:
- Air Quality
- Environment
- EPA
- Open Data
- Public Health
- IoT
- Government Data
- Real-Time Data
title: AQIStation
---
