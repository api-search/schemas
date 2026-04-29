---
description: A sensor measurement from a climate or environmental sensor associated with an HVAC system.
layout: schema
name: SensorReading
properties_list:
- description: Unique identifier for the sensor.
  name: sensor_id
  type: string
- description: Type of sensor measurement.
  name: sensor_type
  type: string
- description: Measured sensor value.
  name: value
  type: number
- description: Unit of the measurement.
  name: unit
  type: string
- description: Physical location of the sensor.
  name: location
  type: string
- description: Whether the sensor is actively used for thermostat control.
  name: in_use
  type: boolean
- description: Timestamp of the reading.
  name: timestamp
  type: string
provider_name: Aircon
provider_slug: aircon
schema_file: json-schema/aircon-sensor-reading-schema.json
slug: aircon-sensor-reading
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aircon/refs/heads/main/json-schema/aircon-sensor-reading-schema.json\",\n  \"title\": \"SensorReading\",\n  \"description\": \"A sensor measurement from a climate or environmental sensor associated with an HVAC system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sensor_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the sensor.\",\n      \"example\": \"sensor-bedroom-01\"\n    },\n    \"sensor_type\": {\n      \"type\": \"string\",\n      \"enum\": [\"temperature\", \"humidity\", \"occupancy\", \"co2\", \"air_quality\", \"pressure\"],\n      \"description\": \"Type of sensor measurement.\",\n      \"example\": \"temperature\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Measured sensor value.\",\n      \"example\": 71.2\n    },\n    \"unit\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"Unit of the measurement.\",\n      \"example\": \"fahrenheit\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Physical location of the sensor.\",\n      \"example\": \"Bedroom\"\n    },\n    \"in_use\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the sensor is actively used for thermostat control.\",\n      \"example\": true\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the reading.\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    }\n  },\n  \"required\": [\"sensor_id\", \"sensor_type\", \"value\", \"timestamp\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aircon/refs/heads/main/json-schema/aircon-sensor-reading-schema.json
tags:
- Air Conditioning
- HVAC
- Climate Control
- IoT
- Smart Home
- Thermostat
- Building Automation
- Energy Management
title: SensorReading
---
