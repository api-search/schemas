---
description: Detailed keys for the location from AccuWeather to aid in weather data retrieval.
layout: schema
name: LocationSettingsInfo
properties_list:
- description: Unique Id created for favorite and recent locations
  name: id
  type: string
- description: AccuWeather Surefind location key for this location.
  name: locationKey
  type: string
- description: Simple name for a location, such as the name of a city
  name: name
  type: string
- description: Full name for a location, such as the name of an Admin or address
  name: longName
  type: string
- description: Name used to display to the user as the placeholder This differece from the LongName since will be sometimes display location name from the AW API (Non-english/direct location key serach)
  name: displayName
  type: string
- description: AccuWeather station code for this location.
  name: stationCode
  type: string
- description: AccuWeather list of supported data sets for this location.
  name: supportedDataSets
  type: array
- description: True if a location supports MinuteCast data.
  name: supportsMinuteCast
  type: boolean
- description: Latitude for a location
  name: latitude
  type: number
- description: Longitude for a location
  name: longitude
  type: number
- description: True if a location supports probabilities on weather events.
  name: supportsEventConfidence
  type: boolean
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-location-settings-info-schema.json
slug: accuweather-location-settings-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-location-settings-info-schema.json\",\n  \"title\": \"LocationSettingsInfo\",\n  \"description\": \"Detailed keys for the location from AccuWeather to aid in weather data retrieval.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Id created for favorite and recent locations\",\n      \"nullable\": true,\n      \"example\": \"50603e3f-5433-4d14-9b5f-01c8cf619d9b\"\n    },\n    \"locationKey\": {\n      \"type\": \"string\",\n      \"description\": \"AccuWeather Surefind location key for this location.\",\n      \"nullable\": true,\n      \"example\": \"328328\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Simple name for a location, such as the name of a city\",\n      \"nullable\": true,\n\
  \      \"example\": \"State Collage\"\n    },\n    \"longName\": {\n      \"type\": \"string\",\n      \"description\": \"Full name for a location, such as the name of an Admin or address\",\n      \"nullable\": true,\n      \"example\": \"385 Science Park Rd, State College, PA\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Name used to display to the user as the placeholder\\r\\nThis differece from the LongName since will be sometimes display location name from\\r\\nthe AW API (Non-english/direct location key serach)\",\n      \"nullable\": true,\n      \"example\": \"385 Science Park Rd, State College, PA or Eureka, CA USA\"\n    },\n    \"stationCode\": {\n      \"type\": \"string\",\n      \"description\": \"AccuWeather station code for this location.\",\n      \"nullable\": true,\n      \"example\": \"EGRB\"\n    },\n    \"supportedDataSets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n     \
  \ \"description\": \"AccuWeather list of supported data sets for this location.\",\n      \"nullable\": true,\n      \"example\": [\n        \"AirQualityCurrentConditions\",\n        \"AirQualityForecasts\",\n        \"Alerts\",\n        \"DailyAirQualityForecast\",\n        \"DailyPollenForecast\",\n        \"ForecastConfidence\",\n        \"FutureRadar\",\n        \"MinuteCast\",\n        \"ProximityNotification-Lightning\",\n        \"Radar\"\n      ]\n    },\n    \"supportsMinuteCast\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if a location supports MinuteCast data.\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"example\": true\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\": \"Latitude for a location\",\n      \"format\": \"double\",\n      \"nullable\": true\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Longitude for a location\",\n      \"format\": \"double\",\n     \
  \ \"nullable\": true\n    },\n    \"supportsEventConfidence\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if a location supports probabilities on weather events.\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"example\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-location-settings-info-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: LocationSettingsInfo
---
