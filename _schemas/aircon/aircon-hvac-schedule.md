---
description: A time-based schedule program for HVAC setpoints and modes.
layout: schema
name: HvacSchedule
properties_list:
- description: Unique identifier for the schedule.
  name: id
  type: string
- description: Human-readable name of the schedule.
  name: name
  type: string
- description: ID of the thermostat this schedule applies to.
  name: thermostat_id
  type: string
- description: Heating setpoint temperature for this schedule period.
  name: heat_setpoint
  type: number
- description: Cooling setpoint temperature for this schedule period.
  name: cool_setpoint
  type: number
- description: Days of the week this schedule applies.
  name: days
  type: array
- description: Start time in HH:MM 24-hour format.
  name: start_time
  type: string
- description: End time in HH:MM 24-hour format.
  name: end_time
  type: string
- description: Whether this schedule is active.
  name: is_enabled
  type: boolean
provider_name: Aircon
provider_slug: aircon
schema_file: json-schema/aircon-hvac-schedule-schema.json
slug: aircon-hvac-schedule
source_filename: aircon-hvac-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aircon/refs/heads/main/json-schema/aircon-hvac-schedule-schema.json\",\n  \"title\": \"HvacSchedule\",\n  \"description\": \"A time-based schedule program for HVAC setpoints and modes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the schedule.\",\n      \"example\": \"schedule-home\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the schedule.\",\n      \"example\": \"Home\"\n    },\n    \"thermostat_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the thermostat this schedule applies to.\",\n      \"example\": \"thermostat-a1b2c3\"\n    },\n    \"heat_setpoint\": {\n      \"type\": \"number\",\n      \"description\": \"Heating setpoint temperature for this schedule period.\"\
  ,\n      \"example\": 68.0\n    },\n    \"cool_setpoint\": {\n      \"type\": \"number\",\n      \"description\": \"Cooling setpoint temperature for this schedule period.\",\n      \"example\": 76.0\n    },\n    \"days\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"monday\", \"tuesday\", \"wednesday\", \"thursday\", \"friday\", \"saturday\", \"sunday\"]\n      },\n      \"description\": \"Days of the week this schedule applies.\",\n      \"example\": [\"monday\", \"tuesday\", \"wednesday\", \"thursday\", \"friday\"]\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"Start time in HH:MM 24-hour format.\",\n      \"example\": \"08:00\"\n    },\n    \"end_time\": {\n      \"type\": \"string\",\n      \"description\": \"End time in HH:MM 24-hour format.\",\n      \"example\": \"17:00\"\n    },\n    \"is_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this schedule is active.\"\
  ,\n      \"example\": true\n    }\n  },\n  \"required\": [\"id\", \"thermostat_id\", \"heat_setpoint\", \"cool_setpoint\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aircon/refs/heads/main/json-schema/aircon-hvac-schedule-schema.json
tags:
- Air Conditioning
- HVAC
- Climate Control
- IoT
- Smart Home
- Thermostat
- Building Automation
- Energy Management
title: HvacSchedule
---
