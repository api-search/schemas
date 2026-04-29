---
description: UserNetwork schema from AccuWeather API
layout: schema
name: UserNetwork
properties_list:
- description: Category of 'network speed' for the user. Eg. 'vhigh'
  name: throughput
  type: string
- description: Name of the network for the user. Eg. 'comcast'
  name: network
  type: string
- description: Type of network for the user. Eg. 'cable'
  name: type
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-user-network-schema.json
slug: accuweather-user-network
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-user-network-schema.json\",\n  \"title\": \"UserNetwork\",\n  \"description\": \"UserNetwork schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"throughput\": {\n      \"type\": \"string\",\n      \"description\": \"Category of 'network speed' for the user. Eg. 'vhigh'\",\n      \"nullable\": true\n    },\n    \"network\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the network for the user. Eg. 'comcast'\",\n      \"nullable\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of network for the user. Eg. 'cable'\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-user-network-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: UserNetwork
---
