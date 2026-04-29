---
description: Goal specification for a navigation episode
layout: schema
name: NavigationGoal
properties_list:
- description: Goal position [x, y, z] in scene coordinates
  name: position
  type: array
- description: Success radius in meters
  name: radius
  type: number
provider_name: AI Habitat
provider_slug: ai-habitat
schema_file: json-schema/ai-habitat-navigation-goal-schema.json
slug: ai-habitat-navigation-goal
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-navigation-goal-schema.json\",\n  \"title\": \"NavigationGoal\",\n  \"description\": \"Goal specification for a navigation episode\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"position\": {\n      \"type\": \"array\",\n      \"description\": \"Goal position [x, y, z] in scene coordinates\",\n      \"items\": {\n        \"type\": \"number\"\n      }\n    },\n    \"radius\": {\n      \"type\": \"number\",\n      \"description\": \"Success radius in meters\",\n      \"example\": 0.2\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ai-habitat/refs/heads/main/json-schema/ai-habitat-navigation-goal-schema.json
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
title: NavigationGoal
---
