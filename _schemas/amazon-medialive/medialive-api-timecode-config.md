---
description: Timecode Config
layout: schema
name: TimecodeConfig
properties_list:
- description: ''
  name: Source
  type: object
- description: ''
  name: SyncThreshold
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-timecode-config-schema.json
slug: medialive-api-timecode-config
source_filename: medialive-api-timecode-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-timecode-config-schema.json\",\n  \"title\": \"TimecodeConfig\",\n  \"description\": \"Timecode Config\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeConfigSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"source\"\n          },\n          \"description\": \"Identifies the source for the timecode that will be associated with the events outputs.\\n-Embedded (embedded): Initialize the output timecode with timecode from the the source.  If no embedded timecode is detected in the source, the system falls back to using \\\"Start at 0\\\" (zerobased).\\n-System Clock (systemclock): Use the UTC time.\\n-Start at 0 (zerobased): The time of the first frame of the event\
  \ will be 00:00:00:00.\"\n        }\n      ]\n    },\n    \"SyncThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max1000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"syncThreshold\"\n          },\n          \"description\": \"Threshold in frames beyond which output timecode is resynchronized to the input timecode. Discrepancies below this threshold are permitted to avoid unnecessary discontinuities in the output timecode. No timecode sync when this is not specified.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-timecode-config-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TimecodeConfig
---
