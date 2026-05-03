---
description: Schema for a SCADA alarm event triggered when a tag value crosses a configured threshold
layout: schema
name: ScadaAlarm
properties_list:
- description: Unique identifier for the alarm instance
  name: alarmId
  type: string
- description: Name or label of the alarm
  name: alarmName
  type: string
- description: Tag ID that triggered the alarm
  name: tagId
  type: string
- description: Type of alarm condition
  name: alarmType
  type: string
- description: Alarm priority level (1=Critical, 2=High, 3=Medium, 4=Low)
  name: priority
  type: integer
- description: Current state of the alarm
  name: state
  type: string
- description: ISO 8601 timestamp when the alarm became active
  name: activeTimestamp
  type: string
- description: ISO 8601 timestamp when the alarm was acknowledged by an operator
  name: acknowledgedTimestamp
  type: string
- description: ISO 8601 timestamp when the alarm condition cleared
  name: clearedTimestamp
  type: string
- description: Tag value at the time the alarm was triggered
  name: triggerValue
  type: number
- description: Alarm limit that was exceeded
  name: limitValue
  type: number
- description: Engineering units of the trigger value
  name: engineeringUnits
  type: string
- description: Human-readable alarm message displayed to operators
  name: message
  type: string
- description: Username of the operator who acknowledged the alarm
  name: acknowledgedBy
  type: string
- description: Process area where the alarm occurred
  name: processArea
  type: string
- description: Operator notes added during alarm acknowledgment
  name: notes
  type: string
provider_name: SCADA
provider_slug: scada
schema_file: json-schema/scada-alarm-schema.json
slug: scada-alarm
source_filename: scada-alarm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scada/main/json-schema/scada-alarm-schema.json\",\n  \"title\": \"ScadaAlarm\",\n  \"description\": \"Schema for a SCADA alarm event triggered when a tag value crosses a configured threshold\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alarmId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the alarm instance\",\n      \"example\": \"ALM-2026-05-02-001\"\n    },\n    \"alarmName\": {\n      \"type\": \"string\",\n      \"description\": \"Name or label of the alarm\",\n      \"example\": \"Reactor Inlet Pressure High-High\"\n    },\n    \"tagId\": {\n      \"type\": \"string\",\n      \"description\": \"Tag ID that triggered the alarm\",\n      \"example\": \"PLANT1.AREA2.PV_101\"\n    },\n    \"alarmType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of alarm condition\",\n      \"enum\"\
  : [\"High-High\", \"High\", \"Low\", \"Low-Low\", \"Rate-of-Change\", \"Deviation\", \"Discrete\", \"Communication\"],\n      \"example\": \"High-High\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Alarm priority level (1=Critical, 2=High, 3=Medium, 4=Low)\",\n      \"minimum\": 1,\n      \"maximum\": 4,\n      \"example\": 1\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the alarm\",\n      \"enum\": [\"Active\", \"Acknowledged\", \"Returned-to-Normal\", \"Shelved\"],\n      \"example\": \"Active\"\n    },\n    \"activeTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the alarm became active\",\n      \"example\": \"2026-05-02T14:35:00.000Z\"\n    },\n    \"acknowledgedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the alarm was acknowledged\
  \ by an operator\"\n    },\n    \"clearedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the alarm condition cleared\"\n    },\n    \"triggerValue\": {\n      \"type\": \"number\",\n      \"description\": \"Tag value at the time the alarm was triggered\",\n      \"example\": 185.3\n    },\n    \"limitValue\": {\n      \"type\": \"number\",\n      \"description\": \"Alarm limit that was exceeded\",\n      \"example\": 180.0\n    },\n    \"engineeringUnits\": {\n      \"type\": \"string\",\n      \"description\": \"Engineering units of the trigger value\",\n      \"example\": \"PSI\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable alarm message displayed to operators\",\n      \"example\": \"CRITICAL: Reactor inlet pressure PV-101 exceeded 180 PSI limit\"\n    },\n    \"acknowledgedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the\
  \ operator who acknowledged the alarm\"\n    },\n    \"processArea\": {\n      \"type\": \"string\",\n      \"description\": \"Process area where the alarm occurred\",\n      \"example\": \"Reactor Section\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Operator notes added during alarm acknowledgment\"\n    }\n  },\n  \"required\": [\"alarmId\", \"tagId\", \"alarmType\", \"priority\", \"state\", \"activeTimestamp\", \"message\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scada/refs/heads/main/json-schema/scada-alarm-schema.json
tags:
- Critical Infrastructure
- ICS
- Industrial Automation
- Industrial IoT
- OT Security
- SCADA
title: ScadaAlarm
---
