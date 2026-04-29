---
description: Sensor observation returned from a simulation step
layout: schema
name: Observation
properties_list:
- description: RGB image array (H x W x 4)
  name: rgb
  type: object
- description: Depth image array (H x W x 1) in meters
  name: depth
  type: object
- description: Semantic segmentation array (H x W x 1) with object instance IDs
  name: semantic
  type: object
- description: GPS coordinates [x, z] relative to start
  name: gps
  type: array
- description: Compass heading in radians
  name: compass
  type: array
provider_name: AI Habitat
provider_slug: ai-habitat
schema_file: json-schema/ai-habitat-observation-schema.json
slug: ai-habitat-observation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-observation-schema.json\",\n  \"title\": \"Observation\",\n  \"description\": \"Sensor observation returned from a simulation step\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rgb\": {\n      \"type\": \"object\",\n      \"description\": \"RGB image array (H x W x 4)\"\n    },\n    \"depth\": {\n      \"type\": \"object\",\n      \"description\": \"Depth image array (H x W x 1) in meters\"\n    },\n    \"semantic\": {\n      \"type\": \"object\",\n      \"description\": \"Semantic segmentation array (H x W x 1) with object instance IDs\"\n    },\n    \"gps\": {\n      \"type\": \"array\",\n      \"description\": \"GPS coordinates [x, z] relative to start\",\n      \"items\": {\n        \"type\": \"number\"\n      }\n    },\n    \"compass\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Compass heading in radians\",\n      \"items\": {\n        \"type\": \"number\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-observation-schema.json
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
title: Observation
---
