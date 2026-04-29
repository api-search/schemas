---
description: Station data including AQI and pollutant readings
layout: schema
name: StationData
properties_list:
- description: Overall Air Quality Index value
  name: aqi
  type: integer
- description: Station ID in AQICN database
  name: idx
  type: integer
- description: ''
  name: city
  type: object
- description: ''
  name: time
  type: object
- description: ''
  name: iaqi
  type: object
- description: ''
  name: forecast
  type: object
- description: Data source attributions
  name: attributions
  type: array
provider_name: Air Quality Programmatic APIs
provider_slug: air-quality-programmatic-apis
schema_file: json-schema/aqicn-station-data-schema.json
slug: aqicn-station-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-station-data-schema.json\",\n  \"title\": \"StationData\",\n  \"description\": \"Station data including AQI and pollutant readings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aqi\": {\n      \"type\": \"integer\",\n      \"description\": \"Overall Air Quality Index value\",\n      \"example\": 45\n    },\n    \"idx\": {\n      \"type\": \"integer\",\n      \"description\": \"Station ID in AQICN database\",\n      \"example\": 8502\n    },\n    \"city\": {\n      \"$ref\": \"#/components/schemas/CityInfo\"\n    },\n    \"time\": {\n      \"$ref\": \"#/components/schemas/TimeInfo\"\n    },\n    \"iaqi\": {\n      \"$ref\": \"#/components/schemas/PollutantData\"\n    },\n    \"forecast\": {\n      \"$ref\": \"#/components/schemas/ForecastData\"\n    },\n    \"attributions\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Data source attributions\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Attribution\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-station-data-schema.json
tags:
- Air Quality
- Environment
- EPA
- Open Data
- Public Health
- IoT
- Government Data
- Real-Time Data
title: StationData
---
