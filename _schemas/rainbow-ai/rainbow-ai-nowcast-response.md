---
description: Schema for the Rainbow.AI Nowcast API response containing minute-by-minute precipitation forecasts
layout: schema
name: Rainbow.AI Nowcast Response
properties_list:
- description: ''
  name: location
  type: object
- description: Array of minute-by-minute precipitation forecasts for up to 4 hours
  name: forecasts
  type: array
- description: ISO 8601 timestamp of the last data update
  name: updated_at
  type: string
provider_name: Rainbow.AI
provider_slug: rainbow-ai
schema_file: json-schema/rainbow-ai-nowcast-response-schema.json
slug: rainbow-ai-nowcast-response
source_filename: rainbow-ai-nowcast-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.rainbow.ai/schemas/nowcast-response\",\n  \"title\": \"Rainbow.AI Nowcast Response\",\n  \"description\": \"Schema for the Rainbow.AI Nowcast API response containing minute-by-minute precipitation forecasts\",\n  \"type\": \"object\",\n  \"required\": [\"location\", \"forecasts\", \"updated_at\"],\n  \"properties\": {\n    \"location\": {\n      \"$ref\": \"#/$defs/Location\"\n    },\n    \"forecasts\": {\n      \"type\": \"array\",\n      \"description\": \"Array of minute-by-minute precipitation forecasts for up to 4 hours\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ForecastPoint\"\n      },\n      \"minItems\": 1,\n      \"maxItems\": 240\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the last data update\"\n    }\n  },\n  \"$defs\": {\n    \"Location\": {\n      \"type\": \"object\"\
  ,\n      \"title\": \"Location\",\n      \"description\": \"Geographic coordinates\",\n      \"required\": [\"lat\", \"lon\"],\n      \"properties\": {\n        \"lat\": {\n          \"type\": \"number\",\n          \"description\": \"Latitude in decimal degrees (-90 to 90)\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"lon\": {\n          \"type\": \"number\",\n          \"description\": \"Longitude in decimal degrees (-180 to 180)\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        }\n      }\n    },\n    \"ForecastPoint\": {\n      \"type\": \"object\",\n      \"title\": \"Forecast Point\",\n      \"description\": \"A single minute precipitation forecast data point\",\n      \"required\": [\"timestamp\", \"precipitation_type\", \"precipitation_intensity\"],\n      \"properties\": {\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp for this\
  \ forecast minute\"\n        },\n        \"precipitation_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of precipitation expected\",\n          \"enum\": [\"none\", \"rain\", \"snow\", \"sleet\", \"freezing_rain\"]\n        },\n        \"precipitation_intensity\": {\n          \"type\": \"number\",\n          \"description\": \"Precipitation intensity in mm/hour\",\n          \"minimum\": 0\n        },\n        \"probability\": {\n          \"type\": \"number\",\n          \"description\": \"Probability of precipitation occurring (0.0 to 1.0)\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rainbow-ai/refs/heads/main/json-schema/rainbow-ai-nowcast-response-schema.json
tags:
- Weather
- Precipitation
- Forecasting
- Nowcast
- Radar
- Tiles
- Geospatial
title: Rainbow.AI Nowcast Response
---
