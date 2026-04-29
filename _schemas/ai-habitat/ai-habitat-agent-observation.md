---
description: Full observation dict returned to an agent after each step
layout: schema
name: AgentObservation
properties_list:
- description: RGB camera observation
  name: rgb
  type: object
- description: Depth camera observation
  name: depth
  type: object
- description: Point goal with GPS/compass sensor
  name: pointgoal_with_gps_compass
  type: object
- description: Object category name for ObjectNav tasks
  name: objectgoal
  type: string
provider_name: AI Habitat
provider_slug: ai-habitat
schema_file: json-schema/ai-habitat-agent-observation-schema.json
slug: ai-habitat-agent-observation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-agent-observation-schema.json\",\n  \"title\": \"AgentObservation\",\n  \"description\": \"Full observation dict returned to an agent after each step\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rgb\": {\n      \"type\": \"object\",\n      \"description\": \"RGB camera observation\"\n    },\n    \"depth\": {\n      \"type\": \"object\",\n      \"description\": \"Depth camera observation\"\n    },\n    \"pointgoal_with_gps_compass\": {\n      \"type\": \"object\",\n      \"description\": \"Point goal with GPS/compass sensor\"\n    },\n    \"objectgoal\": {\n      \"type\": \"string\",\n      \"description\": \"Object category name for ObjectNav tasks\",\n      \"example\": \"chair\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-agent-observation-schema.json
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
title: AgentObservation
---
