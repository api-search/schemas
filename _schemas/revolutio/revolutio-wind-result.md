---
description: Wind hazard analysis result returned by the Revolutio Hazard API per AS/NZS 1170.2 or ASCE 7
layout: schema
name: Revolutio Wind Hazard Analysis Result
properties_list:
- description: Wind region classification (e.g., A0, A1, B, C, D)
  name: region
  type: string
- description: Site wind class (e.g., N1-N6, C1-C3)
  name: class
  type: string
- description: Critical wind direction angle or compass point
  name: criticalDirection
  type: string
- description: Directional terrain category for each wind direction
  name: terrainCategory
  type: object
- description: Directional topographic multiplier class
  name: topographicClass
  type: object
- description: Directional shielding multiplier class
  name: shieldingClass
  type: object
- description: Design wind speed in m/s (metric) or mph (imperial)
  name: windSpeed
  type: number
- description: Applied design standard
  name: standard
  type: string
provider_name: Revolutio
provider_slug: revolutio
schema_file: json-schema/revolutio-wind-result-schema.json
slug: revolutio-wind-result
source_filename: revolutio-wind-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/revolutio/main/json-schema/revolutio-wind-result-schema.json\",\n  \"title\": \"Revolutio Wind Hazard Analysis Result\",\n  \"description\": \"Wind hazard analysis result returned by the Revolutio Hazard API per AS/NZS 1170.2 or ASCE 7\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Wind region classification (e.g., A0, A1, B, C, D)\",\n      \"example\": \"A0\"\n    },\n    \"class\": {\n      \"type\": \"string\",\n      \"description\": \"Site wind class (e.g., N1-N6, C1-C3)\",\n      \"example\": \"N1\"\n    },\n    \"criticalDirection\": {\n      \"type\": \"string\",\n      \"description\": \"Critical wind direction angle or compass point\",\n      \"example\": \"N\"\n    },\n    \"terrainCategory\": {\n      \"type\": \"object\",\n      \"description\": \"Directional terrain\
  \ category for each wind direction\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"topographicClass\": {\n      \"type\": \"object\",\n      \"description\": \"Directional topographic multiplier class\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"shieldingClass\": {\n      \"type\": \"object\",\n      \"description\": \"Directional shielding multiplier class\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"windSpeed\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Design wind speed in m/s (metric) or mph (imperial)\"\n    },\n    \"standard\": {\n      \"type\": \"string\",\n      \"description\": \"Applied design standard\",\n      \"example\": \"AS/NZS 1170.2-2021\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/revolutio/refs/heads/main/json-schema/revolutio-wind-result-schema.json
tags:
- Engineering
- Hazard
- Weather
- Structural Engineering
- Wind Analysis
- Construction
title: Revolutio Wind Hazard Analysis Result
---
