---
description: UserInfo schema from AccuWeather API
layout: schema
name: UserInfo
properties_list:
- description: Unique ID for the user (persistent across sessions)
  name: id
  type: string
- description: Language code set for the product for the user (en-us, en-gb, etc.)
  name: language
  type: string
- description: Country code for the user's location. Eg. US
  name: country
  type: string
- description: Region code for the user's location. Eg. PA
  name: region
  type: string
- description: City for the location
  name: city
  type: string
- description: DMA for the user's location. Eg. 566. Not available outside of the US.
  name: dma
  type: string
- description: Date of the user's first visit. I.e. Cookie creation date
  name: start
  type: string
- description: Valid string of the user's current UTC offset in hh:mm:ss format. Ex. -05:00 or 05:00
  name: offset
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-user-info-schema.json
slug: accuweather-user-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-user-info-schema.json\",\n  \"title\": \"UserInfo\",\n  \"description\": \"UserInfo schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID for the user (persistent across sessions)\",\n      \"nullable\": true\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language code set for the product for the user (en-us, en-gb, etc.)\",\n      \"nullable\": true\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code for the user's location.\\r\\nEg. US\",\n      \"nullable\": true\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Region code for the user's location.\\r\\nEg. PA\",\n      \"nullable\"\
  : true\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City for the location\",\n      \"nullable\": true\n    },\n    \"dma\": {\n      \"type\": \"string\",\n      \"description\": \"DMA for the user's location.\\r\\nEg. 566. Not available outside of the US.\",\n      \"nullable\": true\n    },\n    \"start\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the user's first visit.\\r\\nI.e. Cookie creation date\",\n      \"nullable\": true\n    },\n    \"offset\": {\n      \"type\": \"string\",\n      \"description\": \"Valid string of the user's current UTC offset in hh:mm:ss format.\\r\\nEx. -05:00 or 05:00\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-user-info-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: UserInfo
---
