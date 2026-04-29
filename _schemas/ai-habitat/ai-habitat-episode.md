---
description: A single training/evaluation episode with start and goal specification
layout: schema
name: Episode
properties_list:
- description: Unique episode identifier
  name: episode_id
  type: string
- description: Scene file path for this episode
  name: scene_id
  type: string
- description: Agent starting position [x, y, z]
  name: start_position
  type: array
- description: Agent starting rotation quaternion
  name: start_rotation
  type: array
- description: List of goal specifications
  name: goals
  type: array
- description: Additional episode metadata
  name: info
  type: object
provider_name: AI Habitat
provider_slug: ai-habitat
schema_file: json-schema/ai-habitat-episode-schema.json
slug: ai-habitat-episode
source_filename: ai-habitat-episode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-episode-schema.json\",\n  \"title\": \"Episode\",\n  \"description\": \"A single training/evaluation episode with start and goal specification\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"episode_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique episode identifier\",\n      \"example\": \"ep_001\"\n    },\n    \"scene_id\": {\n      \"type\": \"string\",\n      \"description\": \"Scene file path for this episode\",\n      \"example\": \"data/scene_datasets/hm3d/train/00001/mesh.basis.glb\"\n    },\n    \"start_position\": {\n      \"type\": \"array\",\n      \"description\": \"Agent starting position [x, y, z]\",\n      \"items\": {\n        \"type\": \"number\"\n      }\n    },\n    \"start_rotation\": {\n      \"type\": \"array\",\n      \"description\": \"Agent starting\
  \ rotation quaternion\",\n      \"items\": {\n        \"type\": \"number\"\n      }\n    },\n    \"goals\": {\n      \"type\": \"array\",\n      \"description\": \"List of goal specifications\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"info\": {\n      \"type\": \"object\",\n      \"description\": \"Additional episode metadata\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-episode-schema.json
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
title: Episode
---
