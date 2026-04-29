---
description: Specification for a simulated sensor
layout: schema
name: SensorSpec
properties_list:
- description: Unique sensor identifier
  name: uuid
  type: string
- description: 'Sensor type: COLOR, DEPTH, SEMANTIC, EQUIRECTANGULAR'
  name: sensor_type
  type: string
- description: '[height, width] in pixels'
  name: resolution
  type: array
- description: Sensor position [x, y, z] relative to agent
  name: position
  type: array
- description: Sensor orientation quaternion
  name: orientation
  type: array
- description: Horizontal field of view in degrees
  name: hfov
  type: number
provider_name: AI Habitat
provider_slug: ai-habitat
schema_file: json-schema/ai-habitat-sensor-spec-schema.json
slug: ai-habitat-sensor-spec
source_filename: ai-habitat-sensor-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-sensor-spec-schema.json\",\n  \"title\": \"SensorSpec\",\n  \"description\": \"Specification for a simulated sensor\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique sensor identifier\",\n      \"example\": \"rgb\"\n    },\n    \"sensor_type\": {\n      \"type\": \"string\",\n      \"description\": \"Sensor type: COLOR, DEPTH, SEMANTIC, EQUIRECTANGULAR\",\n      \"example\": \"COLOR\"\n    },\n    \"resolution\": {\n      \"type\": \"array\",\n      \"description\": \"[height, width] in pixels\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"example\": [\n        256,\n        256\n      ]\n    },\n    \"position\": {\n      \"type\": \"array\",\n      \"description\": \"Sensor position [x, y, z]\
  \ relative to agent\",\n      \"items\": {\n        \"type\": \"number\"\n      }\n    },\n    \"orientation\": {\n      \"type\": \"array\",\n      \"description\": \"Sensor orientation quaternion\",\n      \"items\": {\n        \"type\": \"number\"\n      }\n    },\n    \"hfov\": {\n      \"type\": \"number\",\n      \"description\": \"Horizontal field of view in degrees\",\n      \"example\": 90\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-sensor-spec-schema.json
tags:
- Artificial Intelligence
- Simulation
- Embodied AI
- Robotics
- Computer Vision
- Reinforcement Learning
- Machine Learning
- Open Source
- Research
title: SensorSpec
---
