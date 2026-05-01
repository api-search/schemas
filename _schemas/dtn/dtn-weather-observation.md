---
description: Schema representing a weather observation or forecast data point from the DTN Weather API.
layout: schema
name: DTN Weather Observation
properties_list:
- description: Weather station identifier (ICAO, WMO, or DTN identifier)
  name: stationId
  type: string
- description: Human-readable station name
  name: stationName
  type: string
- description: ISO 8601 timestamp of observation
  name: observedAt
  type: string
- description: ''
  name: location
  type: object
- description: Unit system for all measurements
  name: units
  type: string
- description: ''
  name: temperature
  type: object
- description: ''
  name: wind
  type: object
- description: ''
  name: precipitation
  type: object
- description: ''
  name: atmosphere
  type: object
- description: Horizontal visibility in meters (SI) or miles (US)
  name: visibility
  type: number
- description: WMO present weather code (0-99)
  name: weatherSymbol
  type: integer
- description: Total cloud cover percentage
  name: cloudCoverInPercent
  type: number
- description: UV index (0-11+)
  name: uvIndex
  type: number
- description: Soil temperature at surface in degrees Celsius
  name: soilTemperatureInCelsius
  type: number
- description: Potential evapotranspiration in mm (agricultural use)
  name: evapotranspirationInMillimeter
  type: number
provider_name: dtn
provider_slug: dtn
schema_file: json-schema/dtn-weather-observation-schema.json
slug: dtn-weather-observation
source_filename: dtn-weather-observation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://point-observation.weather.mg/schemas/observation\",\n  \"title\": \"DTN Weather Observation\",\n  \"description\": \"Schema representing a weather observation or forecast data point from the DTN Weather API.\",\n  \"type\": \"object\",\n  \"required\": [\"location\"],\n  \"properties\": {\n    \"stationId\": {\n      \"type\": \"string\",\n      \"description\": \"Weather station identifier (ICAO, WMO, or DTN identifier)\",\n      \"examples\": [\"KMSP\", \"KORD\", \"72658\"]\n    },\n    \"stationName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable station name\"\n    },\n    \"observedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of observation\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/GeoLocation\"\n    },\n    \"units\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Unit system for all measurements\",\n      \"enum\": [\"SI\", \"US\"]\n    },\n    \"temperature\": {\n      \"$ref\": \"#/$defs/TemperatureData\"\n    },\n    \"wind\": {\n      \"$ref\": \"#/$defs/WindData\"\n    },\n    \"precipitation\": {\n      \"$ref\": \"#/$defs/PrecipitationData\"\n    },\n    \"atmosphere\": {\n      \"$ref\": \"#/$defs/AtmosphericData\"\n    },\n    \"visibility\": {\n      \"type\": \"number\",\n      \"description\": \"Horizontal visibility in meters (SI) or miles (US)\",\n      \"minimum\": 0\n    },\n    \"weatherSymbol\": {\n      \"type\": \"integer\",\n      \"description\": \"WMO present weather code (0-99)\",\n      \"minimum\": 0,\n      \"maximum\": 99\n    },\n    \"cloudCoverInPercent\": {\n      \"type\": \"number\",\n      \"description\": \"Total cloud cover percentage\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"uvIndex\": {\n      \"type\": \"number\",\n      \"description\": \"UV index (0-11+)\",\n      \"minimum\"\
  : 0\n    },\n    \"soilTemperatureInCelsius\": {\n      \"type\": \"number\",\n      \"description\": \"Soil temperature at surface in degrees Celsius\"\n    },\n    \"evapotranspirationInMillimeter\": {\n      \"type\": \"number\",\n      \"description\": \"Potential evapotranspiration in mm (agricultural use)\",\n      \"minimum\": 0\n    }\n  },\n  \"$defs\": {\n    \"GeoLocation\": {\n      \"type\": \"object\",\n      \"required\": [\"latitude\", \"longitude\"],\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        },\n        \"elevationInMeter\": {\n          \"type\": \"number\",\n          \"description\": \"Elevation above mean sea level in meters\"\n        }\n      }\n    },\n    \"TemperatureData\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"airTemperatureInCelsius\": {\n          \"type\": \"number\",\n          \"description\": \"Air temperature at 2m height in degrees Celsius\"\n        },\n        \"feelsLikeTemperatureInCelsius\": {\n          \"type\": \"number\",\n          \"description\": \"Apparent temperature (heat index or wind chill)\"\n        },\n        \"dewPointInCelsius\": {\n          \"type\": \"number\",\n          \"description\": \"Dew point temperature in degrees Celsius\"\n        },\n        \"maxTemperatureInCelsius\": {\n          \"type\": \"number\",\n          \"description\": \"Maximum temperature over the period\"\n        },\n        \"minTemperatureInCelsius\": {\n          \"type\": \"number\",\n          \"description\": \"Minimum temperature over the period\"\n        },\n        \"wetBulbTemperatureInCelsius\": {\n          \"type\": \"number\",\n          \"description\": \"Wet-bulb temperature in degrees Celsius\"\
  \n        }\n      }\n    },\n    \"WindData\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"windSpeedInMeterPerSecond\": {\n          \"type\": \"number\",\n          \"description\": \"10-minute average wind speed at 10m height\",\n          \"minimum\": 0\n        },\n        \"windDirectionInDegree\": {\n          \"type\": \"number\",\n          \"description\": \"Wind direction in meteorological degrees (0=N, 90=E, 180=S, 270=W)\",\n          \"minimum\": 0,\n          \"maximum\": 360\n        },\n        \"windGustInMeterPerSecond\": {\n          \"type\": \"number\",\n          \"description\": \"Maximum wind gust speed over the period\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"PrecipitationData\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"precipitationAmountInMillimeter\": {\n          \"type\": \"number\",\n          \"description\": \"Total precipitation amount in millimeters\",\n          \"minimum\": 0\n\
  \        },\n        \"precipitationProbabilityInPercent\": {\n          \"type\": \"number\",\n          \"description\": \"Probability of precipitation (0-100%)\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"precipitationTypeCode\": {\n          \"type\": \"integer\",\n          \"description\": \"0=none, 1=rain, 2=snow, 3=sleet, 4=freezing rain, 5=mixed\",\n          \"enum\": [0, 1, 2, 3, 4, 5]\n        },\n        \"snowfallAmountInCentimeter\": {\n          \"type\": \"number\",\n          \"description\": \"New snowfall amount in centimeters\",\n          \"minimum\": 0\n        },\n        \"snowDepthInCentimeter\": {\n          \"type\": \"number\",\n          \"description\": \"Current snow depth on ground in centimeters\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"AtmosphericData\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"pressureInHectopascal\": {\n          \"type\": \"number\",\n          \"description\"\
  : \"Mean sea level pressure in hPa\",\n          \"minimum\": 800,\n          \"maximum\": 1100\n        },\n        \"pressureTendencyInHectopascal\": {\n          \"type\": \"number\",\n          \"description\": \"3-hour pressure tendency in hPa\"\n        },\n        \"relativeHumidityInPercent\": {\n          \"type\": \"number\",\n          \"description\": \"Relative humidity percentage\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dtn/refs/heads/main/json-schema/dtn-weather-observation-schema.json
tags: []
title: DTN Weather Observation
---
