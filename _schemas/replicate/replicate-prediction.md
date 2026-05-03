---
description: A prediction represents a single inference run against a machine learning model on Replicate.
layout: schema
name: Replicate Prediction
properties_list:
- description: The unique identifier for the prediction.
  name: id
  type: string
- description: The ID of the model version used for this prediction.
  name: version
  type:
  - string
  - 'null'
- description: The model owner/name used for official model predictions.
  name: model
  type:
  - string
  - 'null'
- description: URLs associated with the prediction.
  name: urls
  type: object
- description: The current status of the prediction.
  name: status
  type: string
- description: The input provided to the model as a JSON object.
  name: input
  type: object
- description: The output of the prediction. Type depends on the model.
  name: output
  type: object
- description: Error message if the prediction failed.
  name: error
  type:
  - string
  - 'null'
- description: Log output from the prediction.
  name: logs
  type:
  - string
  - 'null'
- description: Performance metrics for the prediction.
  name: metrics
  type: object
- description: Timestamp when the prediction was created.
  name: created_at
  type: string
- description: Timestamp when the prediction started processing.
  name: started_at
  type:
  - string
  - 'null'
- description: Timestamp when the prediction completed.
  name: completed_at
  type:
  - string
  - 'null'
- description: How the prediction was created.
  name: source
  type: string
- description: Webhook URL to receive prediction updates.
  name: webhook
  type:
  - string
  - 'null'
- description: Event types that trigger webhook calls.
  name: webhook_events_filter
  type: array
provider_name: Replicate
provider_slug: replicate
schema_file: json-schema/replicate-prediction-schema.json
slug: replicate-prediction
source_filename: replicate-prediction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/replicate/json-schema/replicate-prediction-schema.json\",\n  \"title\": \"Replicate Prediction\",\n  \"description\": \"A prediction represents a single inference run against a machine learning model on Replicate.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the prediction.\"\n    },\n    \"version\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the model version used for this prediction.\"\n    },\n    \"model\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The model owner/name used for official model predictions.\"\n    },\n    \"urls\": {\n      \"type\": \"object\",\n      \"description\": \"URLs associated with the prediction.\",\n      \"properties\": {\n        \"get\": {\n          \"type\": \"string\"\
  ,\n          \"format\": \"uri\",\n          \"description\": \"URL to poll for prediction status.\"\n        },\n        \"cancel\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to cancel the prediction.\"\n        },\n        \"stream\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for streaming output via SSE.\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"starting\", \"processing\", \"succeeded\", \"failed\", \"canceled\"],\n      \"description\": \"The current status of the prediction.\"\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"The input provided to the model as a JSON object.\"\n    },\n    \"output\": {\n      \"description\": \"The output of the prediction. Type depends on the model.\"\n    },\n    \"error\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"\
  Error message if the prediction failed.\"\n    },\n    \"logs\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Log output from the prediction.\"\n    },\n    \"metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Performance metrics for the prediction.\",\n      \"properties\": {\n        \"predict_time\": {\n          \"type\": \"number\",\n          \"description\": \"Time taken for the prediction in seconds.\"\n        },\n        \"total_time\": {\n          \"type\": \"number\",\n          \"description\": \"Total wall clock time in seconds.\"\n        }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the prediction was created.\"\n    },\n    \"started_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the prediction started processing.\"\n    },\n    \"completed_at\": {\n   \
  \   \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the prediction completed.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"enum\": [\"api\", \"web\"],\n      \"description\": \"How the prediction was created.\"\n    },\n    \"webhook\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"Webhook URL to receive prediction updates.\"\n    },\n    \"webhook_events_filter\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"start\", \"output\", \"logs\", \"completed\"]\n      },\n      \"description\": \"Event types that trigger webhook calls.\"\n    }\n  },\n  \"required\": [\"id\", \"status\", \"created_at\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/json-schema/replicate-prediction-schema.json
tags:
- Artificial Intelligence
- Machine Learning
- Image Generation
- Language Models
- Model Deployment
title: Replicate Prediction
---
