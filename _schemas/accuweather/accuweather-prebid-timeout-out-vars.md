---
description: PrebidTimeoutOutVars schema from AccuWeather API
layout: schema
name: PrebidTimeoutOutVars
properties_list:
- description: ''
  name: prebidTimeout
  type: integer
- description: ''
  name: awxTimeout
  type: integer
- description: ''
  name: bundleUrl
  type: string
- description: ''
  name: bundleId
  type: string
- description: ''
  name: gptEnableSingleRequest
  type: boolean
- description: ''
  name: gptLazyLoading
  type: string
- description: ''
  name: buyItNowSkipGoogleAdManager
  type: boolean
- description: ''
  name: testVariant
  type: string
- description: ''
  name: deviceClass
  type: string
- description: ''
  name: disableInitialAdLoad
  type: boolean
- description: ''
  name: javascriptHead
  type: string
- description: ''
  name: javascriptBody
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-prebid-timeout-out-vars-schema.json
slug: accuweather-prebid-timeout-out-vars
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-prebid-timeout-out-vars-schema.json\",\n  \"title\": \"PrebidTimeoutOutVars\",\n  \"description\": \"PrebidTimeoutOutVars schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prebidTimeout\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"awxTimeout\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"bundleUrl\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"deprecated\": true\n    },\n    \"bundleId\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"gptEnableSingleRequest\": {\n      \"type\": \"boolean\"\n    },\n    \"gptLazyLoading\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"buyItNowSkipGoogleAdManager\": {\n      \"type\": \"boolean\"\
  \n    },\n    \"testVariant\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"deviceClass\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"disableInitialAdLoad\": {\n      \"type\": \"boolean\"\n    },\n    \"javascriptHead\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"javascriptBody\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-prebid-timeout-out-vars-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: PrebidTimeoutOutVars
---
