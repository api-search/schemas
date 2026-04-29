---
description: Individual pollutant AQI values
layout: schema
name: PollutantData
properties_list:
- description: PM2.5 AQI reading
  name: pm25
  type: object
- description: PM10 AQI reading
  name: pm10
  type: object
- description: Nitrogen dioxide AQI reading
  name: no2
  type: object
- description: Ozone AQI reading
  name: o3
  type: object
- description: Sulfur dioxide AQI reading
  name: so2
  type: object
- description: Carbon monoxide AQI reading
  name: co
  type: object
provider_name: Air Quality Programmatic APIs
provider_slug: air-quality-programmatic-apis
schema_file: json-schema/aqicn-pollutant-data-schema.json
slug: aqicn-pollutant-data
source_filename: aqicn-pollutant-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-pollutant-data-schema.json\",\n  \"title\": \"PollutantData\",\n  \"description\": \"Individual pollutant AQI values\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pm25\": {\n      \"type\": \"object\",\n      \"description\": \"PM2.5 AQI reading\",\n      \"properties\": {\n        \"v\": {\n          \"type\": \"number\",\n          \"example\": 45\n        }\n      }\n    },\n    \"pm10\": {\n      \"type\": \"object\",\n      \"description\": \"PM10 AQI reading\",\n      \"properties\": {\n        \"v\": {\n          \"type\": \"number\",\n          \"example\": 32\n        }\n      }\n    },\n    \"no2\": {\n      \"type\": \"object\",\n      \"description\": \"Nitrogen dioxide AQI reading\",\n      \"properties\": {\n        \"v\": {\n          \"type\": \"number\",\n\
  \          \"example\": 12\n        }\n      }\n    },\n    \"o3\": {\n      \"type\": \"object\",\n      \"description\": \"Ozone AQI reading\",\n      \"properties\": {\n        \"v\": {\n          \"type\": \"number\",\n          \"example\": 28\n        }\n      }\n    },\n    \"so2\": {\n      \"type\": \"object\",\n      \"description\": \"Sulfur dioxide AQI reading\",\n      \"properties\": {\n        \"v\": {\n          \"type\": \"number\",\n          \"example\": 5\n        }\n      }\n    },\n    \"co\": {\n      \"type\": \"object\",\n      \"description\": \"Carbon monoxide AQI reading\",\n      \"properties\": {\n        \"v\": {\n          \"type\": \"number\",\n          \"example\": 8\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-quality-programmatic-apis/refs/heads/main/json-schema/aqicn-pollutant-data-schema.json
tags:
- Air Quality
- Environment
- EPA
- Open Data
- Public Health
- IoT
- Government Data
- Real-Time Data
title: PollutantData
---
