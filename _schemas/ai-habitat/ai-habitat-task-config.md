---
description: Habitat-Lab task configuration
layout: schema
name: TaskConfig
properties_list:
- description: Task type string identifier
  name: type
  type: string
- description: Maximum steps per episode
  name: max_episode_steps
  type: integer
- description: List of measurement names to compute
  name: measurements
  type: array
- description: Available action space configuration
  name: actions
  type: object
- description: UUID of the goal sensor
  name: goal_sensor_uuid
  type: string
provider_name: AI Habitat
provider_slug: ai-habitat
schema_file: json-schema/ai-habitat-task-config-schema.json
slug: ai-habitat-task-config
source_filename: ai-habitat-task-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-task-config-schema.json\",\n  \"title\": \"TaskConfig\",\n  \"description\": \"Habitat-Lab task configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Task type string identifier\",\n      \"example\": \"ObjectNav-v1\"\n    },\n    \"max_episode_steps\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum steps per episode\",\n      \"example\": 500\n    },\n    \"measurements\": {\n      \"type\": \"array\",\n      \"description\": \"List of measurement names to compute\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"actions\": {\n      \"type\": \"object\",\n      \"description\": \"Available action space configuration\"\n    },\n    \"goal_sensor_uuid\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"UUID of the goal sensor\",\n      \"example\": \"pointgoal\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-task-config-schema.json
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
title: TaskConfig
---
