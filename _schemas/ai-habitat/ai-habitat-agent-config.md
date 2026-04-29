---
description: Configuration for an agent in the simulation
layout: schema
name: AgentConfig
properties_list:
- description: Agent height in meters
  name: height
  type: number
- description: Agent radius in meters for collision
  name: radius
  type: number
- description: List of sensor specs attached to agent
  name: sensor_specifications
  type: array
- description: Discrete action space mapping action names to ActionSpec
  name: action_space
  type: object
- description: 'Agent body type: LocoBot, FetchRobot, Franka, AlienGo'
  name: body_type
  type: string
provider_name: AI Habitat
provider_slug: ai-habitat
schema_file: json-schema/ai-habitat-agent-config-schema.json
slug: ai-habitat-agent-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-agent-config-schema.json\",\n  \"title\": \"AgentConfig\",\n  \"description\": \"Configuration for an agent in the simulation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"height\": {\n      \"type\": \"number\",\n      \"description\": \"Agent height in meters\",\n      \"example\": 1.5\n    },\n    \"radius\": {\n      \"type\": \"number\",\n      \"description\": \"Agent radius in meters for collision\",\n      \"example\": 0.1\n    },\n    \"sensor_specifications\": {\n      \"type\": \"array\",\n      \"description\": \"List of sensor specs attached to agent\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"action_space\": {\n      \"type\": \"object\",\n      \"description\": \"Discrete action space mapping action names to ActionSpec\"\n    },\n    \"body_type\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Agent body type: LocoBot, FetchRobot, Franka, AlienGo\",\n      \"example\": \"LocoBot\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-agent-config-schema.json
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
title: AgentConfig
---
