---
description: Configuration for the Habitat-Sim simulator instance
layout: schema
name: SimulatorConfig
properties_list:
- description: Path to the 3D scene file (.glb, .ply)
  name: scene_id
  type: string
- description: Default agent index
  name: default_agent_id
  type: integer
- description: List of sensor configurations
  name: sensor_specifications
  type: array
- description: Physics engine to use
  name: physics_simulation_library
  type: string
- description: GPU device ID for rendering
  name: gpu_device_id
  type: integer
- description: Random seed for reproducibility
  name: random_seed
  type: integer
- description: Enable physics simulation
  name: enable_physics
  type: boolean
provider_name: AI Habitat
provider_slug: ai-habitat
schema_file: json-schema/ai-habitat-simulator-config-schema.json
slug: ai-habitat-simulator-config
source_filename: ai-habitat-simulator-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-simulator-config-schema.json\",\n  \"title\": \"SimulatorConfig\",\n  \"description\": \"Configuration for the Habitat-Sim simulator instance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scene_id\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the 3D scene file (.glb, .ply)\",\n      \"example\": \"data/scene_datasets/habitat-test-scenes/apartment_1.glb\"\n    },\n    \"default_agent_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Default agent index\",\n      \"example\": 0\n    },\n    \"sensor_specifications\": {\n      \"type\": \"array\",\n      \"description\": \"List of sensor configurations\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"physics_simulation_library\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Physics engine to use\",\n      \"example\": \"BulletPhysics\"\n    },\n    \"gpu_device_id\": {\n      \"type\": \"integer\",\n      \"description\": \"GPU device ID for rendering\",\n      \"example\": 0\n    },\n    \"random_seed\": {\n      \"type\": \"integer\",\n      \"description\": \"Random seed for reproducibility\",\n      \"example\": 1\n    },\n    \"enable_physics\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable physics simulation\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-simulator-config-schema.json
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
title: SimulatorConfig
---
