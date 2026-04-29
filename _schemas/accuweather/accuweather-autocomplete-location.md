---
description: A location that can be used to plot on a map.
layout: schema
name: AutocompleteLocation
properties_list:
- description: Type of location, eg. address or postalcode
  name: locationType
  type: string
- description: City name of the location, usually used for display purposes when sourcing weather data.
  name: city
  type: string
- description: The admin code for the location.
  name: adminCode
  type: string
- description: County code for the location.
  name: countryCode
  type: string
- description: Postal Code of the location, usually used for display purposes when sourcing weather data.
  name: postalCode
  type: string
- description: City name of the location, usually used for display purposes when sourcing weather data.
  name: position
  type: array
- description: Editable name of the location to display to the user.
  name: name
  type: string
- description: Longer name of the location to display to the user, typically the full address.
  name: longName
  type: string
- description: Detailed keys for the location from AccuWeather to aid in weather data retrieval.
  name: locationSettingsInfo
  type: object
- description: The parent provider of the location.
  name: source
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-autocomplete-location-schema.json
slug: accuweather-autocomplete-location
source_filename: accuweather-autocomplete-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-autocomplete-location-schema.json\",\n  \"title\": \"AutocompleteLocation\",\n  \"description\": \"A location that can be used to plot on a map.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"locationType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of location, eg. address or postalcode\",\n      \"nullable\": true,\n      \"example\": \"address\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name of the location, usually used for display purposes when sourcing weather data.\",\n      \"nullable\": true,\n      \"example\": \"London\"\n    },\n    \"adminCode\": {\n      \"type\": \"string\",\n      \"description\": \"The admin code for the location.\",\n      \"nullable\": true,\n      \"example\": \"PA\"\n    },\n    \"countryCode\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"County code for the location.\",\n      \"nullable\": true,\n      \"example\": \"US\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal Code of the location, usually used for display purposes when sourcing weather data.\",\n      \"nullable\": true\n    },\n    \"position\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"number\",\n        \"format\": \"double\"\n      },\n      \"description\": \"City name of the location, usually used for display purposes when sourcing weather data.\",\n      \"nullable\": true,\n      \"example\": [\n        51.50032,\n        -0.145433\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Editable name of the location to display to the user.\",\n      \"nullable\": true,\n      \"example\": \"Buckingham Palace\"\n    },\n    \"longName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Longer name of the location to display to the user, typically the full address.\",\n      \"nullable\": true,\n      \"example\": \"Buckingham Palace, Westminster, London, Greater London GBR\"\n    },\n    \"locationSettingsInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique Id created for favorite and recent locations\",\n          \"nullable\": true,\n          \"example\": \"50603e3f-5433-4d14-9b5f-01c8cf619d9b\"\n        },\n        \"locationKey\": {\n          \"type\": \"string\",\n          \"description\": \"AccuWeather Surefind location key for this location.\",\n          \"nullable\": true,\n          \"example\": \"328328\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Simple name for a location, such as the name of a city\",\n          \"nullable\": true,\n          \"example\": \"State Collage\"\n        },\n        \"\
  longName\": {\n          \"type\": \"string\",\n          \"description\": \"Full name for a location, such as the name of an Admin or address\",\n          \"nullable\": true,\n          \"example\": \"385 Science Park Rd, State College, PA\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"Name used to display to the user as the placeholder\\r\\nThis differece from the LongName since will be sometimes display location name from\\r\\nthe AW API (Non-english/direct location key serach)\",\n          \"nullable\": true,\n          \"example\": \"385 Science Park Rd, State College, PA or Eureka, CA USA\"\n        },\n        \"stationCode\": {\n          \"type\": \"string\",\n          \"description\": \"AccuWeather station code for this location.\",\n          \"nullable\": true,\n          \"example\": \"EGRB\"\n        },\n        \"supportedDataSets\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\"\
  : \"string\"\n          },\n          \"description\": \"AccuWeather list of supported data sets for this location.\",\n          \"nullable\": true,\n          \"example\": [\n            \"AirQualityCurrentConditions\",\n            \"AirQualityForecasts\",\n            \"Alerts\",\n            \"DailyAirQualityForecast\",\n            \"DailyPollenForecast\",\n            \"ForecastConfidence\",\n            \"FutureRadar\",\n            \"MinuteCast\",\n            \"ProximityNotification-Lightning\",\n            \"Radar\"\n          ]\n        },\n        \"supportsMinuteCast\": {\n          \"type\": \"boolean\",\n          \"description\": \"True if a location supports MinuteCast data.\",\n          \"nullable\": true,\n          \"readOnly\": true,\n          \"example\": true\n        },\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"Latitude for a location\",\n          \"format\": \"double\",\n          \"nullable\": true\n        },\n\
  \        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"Longitude for a location\",\n          \"format\": \"double\",\n          \"nullable\": true\n        },\n        \"supportsEventConfidence\": {\n          \"type\": \"boolean\",\n          \"description\": \"True if a location supports probabilities on weather events.\",\n          \"nullable\": true,\n          \"readOnly\": true,\n          \"example\": true\n        }\n      },\n      \"additionalProperties\": false,\n      \"description\": \"Detailed keys for the location from AccuWeather to aid in weather data retrieval.\"\n    },\n    \"source\": {\n      \"enum\": [\n        \"AccuWeather\",\n        \"Radar\",\n        \"Unknown\"\n      ],\n      \"type\": \"string\",\n      \"description\": \"The parent provider of the location.\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-autocomplete-location-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: AutocompleteLocation
---
