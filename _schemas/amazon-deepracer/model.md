---
description: A reinforcement learning model trained for DeepRacer autonomous racing.
layout: schema
name: Model
properties_list:
- description: The ARN uniquely identifying the reinforcement learning model.
  name: modelArn
  type: string
- description: The display name of the model.
  name: modelName
  type: string
- description: Timestamp when the model was created.
  name: creationTime
  type: string
- description: Timestamp when the model was last updated.
  name: lastModifiedTime
  type: string
- description: Current status of the model.
  name: modelStatus
  type: string
- description: ARN of the SageMaker training job that produced this model.
  name: trainingJobArn
  type: string
- description: Python reward function code used during training.
  name: rewardFunction
  type: string
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
schema_file: json-schema/model-schema.json
slug: model
source_filename: model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deepracer/json-schema/model-schema.json\",\n  \"title\": \"Model\",\n  \"description\": \"A reinforcement learning model trained for DeepRacer autonomous racing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"modelArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN uniquely identifying the reinforcement learning model.\"\n    },\n    \"modelName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the model.\"\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the model was created.\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the model was last updated.\"\n    },\n    \"modelStatus\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Current status of the model.\",\n      \"enum\": [\n        \"TRAINING\",\n        \"READY\",\n        \"FAILED\",\n        \"STOPPED\"\n      ]\n    },\n    \"trainingJobArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the SageMaker training job that produced this model.\"\n    },\n    \"rewardFunction\": {\n      \"type\": \"string\",\n      \"description\": \"Python reward function code used during training.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/json-schema/model-schema.json
tags:
- Autonomous Vehicles
- Machine Learning
- Reinforcement Learning
- Robotics
title: Model
---
