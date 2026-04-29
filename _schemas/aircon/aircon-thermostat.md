---
description: Represents the state and configuration of a smart thermostat or HVAC control unit.
layout: schema
name: Thermostat
properties_list:
- description: Unique identifier for the thermostat device.
  name: id
  type: string
- description: Human-readable name of the thermostat.
  name: name
  type: string
- description: Current measured temperature in degrees.
  name: current_temperature
  type: number
- description: Target temperature setpoint.
  name: target_temperature
  type: number
- description: Unit of temperature measurement.
  name: temperature_unit
  type: string
- description: Current HVAC operating mode.
  name: hvac_mode
  type: string
- description: Current HVAC operation status.
  name: hvac_status
  type: string
- description: Fan operation mode.
  name: fan_mode
  type: string
- description: Current relative humidity percentage.
  name: humidity
  type: number
- description: Target relative humidity percentage.
  name: target_humidity
  type: number
- description: Whether the thermostat is currently online.
  name: is_online
  type: boolean
- description: Physical location or room of the thermostat.
  name: location
  type: string
- description: Thermostat model identifier.
  name: model
  type: string
- description: Current firmware version of the device.
  name: firmware_version
  type: string
- description: Timestamp of the last status update.
  name: last_updated
  type: string
provider_name: Aircon
provider_slug: aircon
schema_file: json-schema/aircon-thermostat-schema.json
slug: aircon-thermostat
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aircon/refs/heads/main/json-schema/aircon-thermostat-schema.json\",\n  \"title\": \"Thermostat\",\n  \"description\": \"Represents the state and configuration of a smart thermostat or HVAC control unit.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the thermostat device.\",\n      \"example\": \"thermostat-a1b2c3\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the thermostat.\",\n      \"example\": \"Living Room Thermostat\"\n    },\n    \"current_temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Current measured temperature in degrees.\",\n      \"example\": 72.5\n    },\n    \"target_temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Target temperature\
  \ setpoint.\",\n      \"example\": 70.0\n    },\n    \"temperature_unit\": {\n      \"type\": \"string\",\n      \"enum\": [\"celsius\", \"fahrenheit\"],\n      \"description\": \"Unit of temperature measurement.\",\n      \"example\": \"fahrenheit\"\n    },\n    \"hvac_mode\": {\n      \"type\": \"string\",\n      \"enum\": [\"off\", \"heat\", \"cool\", \"auto\", \"fan_only\", \"dry\"],\n      \"description\": \"Current HVAC operating mode.\",\n      \"example\": \"cool\"\n    },\n    \"hvac_status\": {\n      \"type\": \"string\",\n      \"enum\": [\"idle\", \"heating\", \"cooling\", \"fan\", \"off\"],\n      \"description\": \"Current HVAC operation status.\",\n      \"example\": \"cooling\"\n    },\n    \"fan_mode\": {\n      \"type\": \"string\",\n      \"enum\": [\"auto\", \"on\", \"circulate\", \"low\", \"medium\", \"high\"],\n      \"description\": \"Fan operation mode.\",\n      \"example\": \"auto\"\n    },\n    \"humidity\": {\n      \"type\": \"number\",\n      \"minimum\"\
  : 0,\n      \"maximum\": 100,\n      \"description\": \"Current relative humidity percentage.\",\n      \"example\": 45.0\n    },\n    \"target_humidity\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Target relative humidity percentage.\",\n      \"example\": 50.0\n    },\n    \"is_online\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the thermostat is currently online.\",\n      \"example\": true\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Physical location or room of the thermostat.\",\n      \"example\": \"Living Room\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Thermostat model identifier.\",\n      \"example\": \"ecobee4\"\n    },\n    \"firmware_version\": {\n      \"type\": \"string\",\n      \"description\": \"Current firmware version of the device.\",\n      \"example\": \"4.8.7.132\"\n    },\n    \"last_updated\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last status update.\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    }\n  },\n  \"required\": [\"id\", \"hvac_mode\", \"current_temperature\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aircon/refs/heads/main/json-schema/aircon-thermostat-schema.json
tags:
- Air Conditioning
- HVAC
- Climate Control
- IoT
- Smart Home
- Thermostat
- Building Automation
- Energy Management
title: Thermostat
---
