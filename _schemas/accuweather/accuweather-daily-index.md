---
description: DailyIndex schema from AccuWeather API
layout: schema
name: DailyIndex
properties_list:
- description: ''
  name: indexName
  type: string
- description: ''
  name: indexType
  type: string
- description: ''
  name: days
  type: array
- description: ''
  name: activityType
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-daily-index-schema.json
slug: accuweather-daily-index
source_filename: accuweather-daily-index-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-daily-index-schema.json\",\n  \"title\": \"DailyIndex\",\n  \"description\": \"DailyIndex schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"indexName\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"indexType\": {\n      \"enum\": [\n        \"Unknown\",\n        \"Running\",\n        \"Jogging\",\n        \"Hiking\",\n        \"Biking\",\n        \"Golf\",\n        \"Tennis\",\n        \"Skateboarding\",\n        \"Concert\",\n        \"KiteFlyingForecast\",\n        \"BeachAndPool\",\n        \"Sailing\",\n        \"Stargazing\",\n        \"FishingForecast\",\n        \"Construction\",\n        \"Skiing\",\n        \"Heart\",\n        \"Mosquito\",\n        \"Dust\",\n        \"SnowDays\",\n        \"Hunting\",\n        \"ArthritisDay\"\
  ,\n        \"ArthritisNight\",\n        \"Asthma\",\n        \"BBQ\",\n        \"CommonColdForecast\",\n        \"Flu\",\n        \"Migraine\",\n        \"LawnMowing\",\n        \"Outdoor\",\n        \"Sinus\",\n        \"Flying\",\n        \"FieldReadiness\",\n        \"GrassGrowing\",\n        \"SoilMoisture\",\n        \"SchoolBusStop\",\n        \"HomeEnergy\",\n        \"FuelEconomy\",\n        \"Composting\",\n        \"ShoppingForecast\",\n        \"Driving\",\n        \"Thirst\",\n        \"Frizz\",\n        \"DogWalking\",\n        \"COPD\",\n        \"IndoorPest\",\n        \"OutdoorPest\",\n        \"AccuLumenBrightness\",\n        \"MorningExercise\",\n        \"Clothing\",\n        \"CommonCold\",\n        \"Comfort\",\n        \"CarWashing\",\n        \"HeatStroke\",\n        \"UVIntensity\",\n        \"ClothesDrying\",\n        \"AirPollution\",\n        \"Tourism\",\n        \"AirConditioning\",\n        \"Fishing\",\n        \"SunProtection\",\n        \"Shopping\",\n\
  \        \"Rowing\",\n        \"Traffic\",\n        \"RoadConditions\",\n        \"Umbrella\",\n        \"HairDressing\",\n        \"NightLife\",\n        \"Beer\",\n        \"KiteFlying\",\n        \"Makeup\",\n        \"WindChills\",\n        \"Mood\",\n        \"Exercise\",\n        \"Dating\",\n        \"Allergy\",\n        \"Beach\",\n        \"Sunglasses\",\n        \"ShortPhrase\",\n        \"Hypertension\",\n        \"Dryness\",\n        \"ApparentTemperature\",\n        \"PolutionPrevention\",\n        \"FoodPoisoning\",\n        \"WindChillDescending\",\n        \"Heat\",\n        \"Discomfort\",\n        \"UVDescending\",\n        \"PipeFreeze\",\n        \"AtmosphericDispersion\",\n        \"HeatSensitivityGeneral\",\n        \"HeatSensitivityElderly\",\n        \"HeatSensitivityChildren\",\n        \"HeatSensitivityOutdoorWorking\",\n        \"HeatSensitivityFarming\",\n        \"HeatSensitivityGreenhouse\",\n        \"HeatSensitivityVulnerableResidential\",\n        \"AsthmaAndLungDisorder\"\
  ,\n        \"Stroke\",\n        \"SkinSensitivity\",\n        \"CommonColdDescending\",\n        \"TreePollenLevels\",\n        \"PinePollen\",\n        \"WeedPollenLevels\",\n        \"Arthritis\",\n        \"OutdoorHomeGarden\",\n        \"SoilHomeGarden\",\n        \"FieldHomeGarden\",\n        \"UV\",\n        \"TreePollen\",\n        \"RagweedPollen\",\n        \"MoldPollen\",\n        \"GrassPollen\",\n        \"AirQuality\",\n        \"FlightDelay\",\n        \"IndoorActivity\"\n      ],\n      \"type\": \"string\"\n    },\n    \"days\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"dayOfWeek\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"shortDayOfWeek\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"fullDayOfWeek\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n   \
  \       \"epoch\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\",\n            \"nullable\": true\n          },\n          \"dateTime\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"displayDate\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"longDisplayDate\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"value\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          },\n          \"color\": {\n            \"type\": \"string\",\n            \"nullable\": true\n          }\n        },\n        \"additionalProperties\": false\n      },\n      \"nullable\": true\n    },\n    \"activityType\": {\n      \"enum\": [\n        \"Allergies\",\n        \"Health\",\n        \"OutdoorActivities\"\
  ,\n        \"TravelCommute\",\n        \"HomeGarden\",\n        \"Pests\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-daily-index-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: DailyIndex
---
