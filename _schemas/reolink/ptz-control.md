---
description: Pan-tilt-zoom control parameters for the PtzCtrl command supporting directional movement, zoom, focus, and preset navigation.
layout: schema
name: Reolink PTZ Control
properties_list:
- description: Camera channel number (starting from 0)
  name: channel
  type: integer
- description: PTZ operation to perform
  name: op
  type: string
- description: Movement speed from 1 (slowest) to 64 (fastest)
  name: speed
  type: integer
- description: Preset position ID used with the ToPos operation
  name: id
  type: integer
provider_name: Reolink
provider_slug: reolink
schema_file: json-schema/ptz-control.json
slug: ptz-control
source_filename: ptz-control.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"ptz-control.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Reolink PTZ Control\",\n  \"description\": \"Pan-tilt-zoom control parameters for the PtzCtrl command supporting directional movement, zoom, focus, and preset navigation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel\": {\n      \"type\": \"integer\",\n      \"description\": \"Camera channel number (starting from 0)\",\n      \"minimum\": 0\n    },\n    \"op\": {\n      \"type\": \"string\",\n      \"description\": \"PTZ operation to perform\",\n      \"enum\": [\n        \"Stop\",\n        \"Left\",\n        \"Right\",\n        \"Up\",\n        \"Down\",\n        \"LeftUp\",\n        \"LeftDown\",\n        \"RightUp\",\n        \"RightDown\",\n        \"ZoomInc\",\n        \"ZoomDec\",\n        \"FocusInc\",\n        \"FocusDec\",\n        \"ToPos\",\n        \"Auto\"\n      ]\n    },\n    \"speed\": {\n      \"type\": \"integer\",\n     \
  \ \"description\": \"Movement speed from 1 (slowest) to 64 (fastest)\",\n      \"minimum\": 1,\n      \"maximum\": 64\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Preset position ID used with the ToPos operation\",\n      \"minimum\": 0\n    }\n  },\n  \"required\": [\"channel\", \"op\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/json-schema/ptz-control.json
tags:
- IoT
- Security Cameras
- Surveillance
- Smart Home
- AI Detection
title: Reolink PTZ Control
---
