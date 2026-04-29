---
description: Energy consumption and runtime report for an HVAC system over a time period.
layout: schema
name: EnergyReport
properties_list:
- description: ID of the thermostat this report covers.
  name: thermostat_id
  type: string
- description: Start of the reporting period.
  name: period_start
  type: string
- description: End of the reporting period.
  name: period_end
  type: string
- description: Total minutes the heating system ran.
  name: heating_runtime_minutes
  type: integer
- description: Total minutes the cooling system ran.
  name: cooling_runtime_minutes
  type: integer
- description: Total minutes the fan ran independently.
  name: fan_runtime_minutes
  type: integer
- description: Estimated energy consumption in kilowatt-hours.
  name: estimated_kwh
  type: number
- description: Average indoor temperature during the period.
  name: average_indoor_temp
  type: number
- description: Average outdoor temperature during the period.
  name: average_outdoor_temp
  type: number
provider_name: Aircon
provider_slug: aircon
schema_file: json-schema/aircon-energy-report-schema.json
slug: aircon-energy-report
source_filename: aircon-energy-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aircon/refs/heads/main/json-schema/aircon-energy-report-schema.json\",\n  \"title\": \"EnergyReport\",\n  \"description\": \"Energy consumption and runtime report for an HVAC system over a time period.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thermostat_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the thermostat this report covers.\",\n      \"example\": \"thermostat-a1b2c3\"\n    },\n    \"period_start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start of the reporting period.\",\n      \"example\": \"2026-04-01T00:00:00Z\"\n    },\n    \"period_end\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"End of the reporting period.\",\n      \"example\": \"2026-04-30T23:59:59Z\"\n    },\n    \"heating_runtime_minutes\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Total minutes the heating system ran.\",\n      \"example\": 120\n    },\n    \"cooling_runtime_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total minutes the cooling system ran.\",\n      \"example\": 480\n    },\n    \"fan_runtime_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total minutes the fan ran independently.\",\n      \"example\": 60\n    },\n    \"estimated_kwh\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated energy consumption in kilowatt-hours.\",\n      \"example\": 45.2\n    },\n    \"average_indoor_temp\": {\n      \"type\": \"number\",\n      \"description\": \"Average indoor temperature during the period.\",\n      \"example\": 71.5\n    },\n    \"average_outdoor_temp\": {\n      \"type\": \"number\",\n      \"description\": \"Average outdoor temperature during the period.\",\n      \"example\": 82.3\n    }\n  },\n  \"required\": [\"thermostat_id\"\
  , \"period_start\", \"period_end\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aircon/refs/heads/main/json-schema/aircon-energy-report-schema.json
tags:
- Air Conditioning
- HVAC
- Climate Control
- IoT
- Smart Home
- Thermostat
- Building Automation
- Energy Management
title: EnergyReport
---
