---
description: Schema for a Rockwell FactoryTalk Optix tag (process variable), representing a named data point in an industrial automation system.
layout: schema
name: Rockwell FactoryTalk Tag
properties_list:
- description: Fully qualified tag name (may use dot notation for nested tags)
  name: name
  type: string
- description: Human-readable display name
  name: displayName
  type: string
- description: Tag description
  name: description
  type: string
- description: Tag data type
  name: dataType
  type: string
- description: Unit of measure (e.g., RPM, °C, bar, m/s)
  name: engineeringUnit
  type: string
- description: True if the tag cannot be written via the API
  name: readOnly
  type: boolean
- description: True if alarm conditions are configured for this tag
  name: alarmEnabled
  type: boolean
- description: Deadband value for filtering minor value changes
  name: deadband
  type:
  - number
  - 'null'
- description: ''
  name: currentValue
  type: object
provider_name: rockwell-factorytalk
provider_slug: rockwell-factorytalk
schema_file: json-schema/rockwell-factorytalk-tag-schema.json
slug: rockwell-factorytalk-tag
source_filename: rockwell-factorytalk-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/rockwell-factorytalk/json-schema/rockwell-factorytalk-tag-schema.json\",\n  \"title\": \"Rockwell FactoryTalk Tag\",\n  \"description\": \"Schema for a Rockwell FactoryTalk Optix tag (process variable), representing a named data point in an industrial automation system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified tag name (may use dot notation for nested tags)\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Tag description\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Bool\", \"Int16\", \"Int32\", \"Int64\", \"UInt16\", \"UInt32\", \"UInt64\", \"Float\", \"Double\", \"String\", \"\
  DateTime\"],\n      \"description\": \"Tag data type\"\n    },\n    \"engineeringUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure (e.g., RPM, °C, bar, m/s)\"\n    },\n    \"readOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the tag cannot be written via the API\"\n    },\n    \"alarmEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if alarm conditions are configured for this tag\"\n    },\n    \"deadband\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Deadband value for filtering minor value changes\"\n    },\n    \"currentValue\": {\n      \"$ref\": \"#/$defs/TagValue\"\n    }\n  },\n  \"required\": [\"name\", \"dataType\"],\n  \"$defs\": {\n    \"TagValue\": {\n      \"type\": \"object\",\n      \"description\": \"Current tag value with timestamp and quality\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"value\": {\n     \
  \     \"description\": \"Current value (type matches tag dataType)\"\n        },\n        \"quality\": {\n          \"type\": \"string\",\n          \"enum\": [\"GOOD\", \"BAD\", \"UNCERTAIN\", \"COMM_FAILURE\"],\n          \"description\": \"Data quality status\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp of the current value\"\n        }\n      },\n      \"required\": [\"timestamp\", \"quality\"]\n    }\n  },\n  \"examples\": [\n    {\n      \"name\": \"Conveyor1.Speed\",\n      \"displayName\": \"Conveyor 1 Speed\",\n      \"description\": \"Conveyor belt 1 speed in meters per minute\",\n      \"dataType\": \"Float\",\n      \"engineeringUnit\": \"m/min\",\n      \"readOnly\": false,\n      \"alarmEnabled\": true,\n      \"deadband\": 0.5,\n      \"currentValue\": {\n        \"name\": \"Conveyor1.Speed\",\n        \"value\": 45.2,\n        \"quality\": \"GOOD\",\n        \"timestamp\"\
  : \"2026-03-18T14:32:00Z\"\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rockwell-factorytalk/refs/heads/main/json-schema/rockwell-factorytalk-tag-schema.json
tags: []
title: Rockwell FactoryTalk Tag
---
