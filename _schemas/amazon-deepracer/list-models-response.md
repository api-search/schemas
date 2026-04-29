---
description: Response containing a list of reinforcement learning models.
layout: schema
name: ListModelsResponse
properties_list:
- description: List of reinforcement learning models.
  name: models
  type: array
- description: Token for retrieving the next page of results.
  name: nextToken
  type: string
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
schema_file: json-schema/list-models-response-schema.json
slug: list-models-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deepracer/json-schema/list-models-response-schema.json\",\n  \"title\": \"ListModelsResponse\",\n  \"description\": \"Response containing a list of reinforcement learning models.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"models\": {\n      \"type\": \"array\",\n      \"description\": \"List of reinforcement learning models.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for retrieving the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/json-schema/list-models-response-schema.json
tags:
- Autonomous Vehicles
- AWS
- Machine Learning
- Reinforcement Learning
- Robotics
title: ListModelsResponse
---
