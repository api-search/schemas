---
description: AI-generated predictive maintenance forecast from Baker Hughes BHC3 AI Suite.
layout: schema
name: Prediction
properties_list:
- description: Unique identifier for the prediction.
  name: predictionId
  type: string
- description: Identifier of the asset this prediction applies to.
  name: assetId
  type: string
- description: Category of prediction.
  name: predictionType
  type: string
- description: Probability of failure in the next prediction window (0.0 to 1.0).
  name: failureProbability
  type: number
- description: Estimated time until failure expressed as ISO 8601 duration (e.g., P7D for 7 days).
  name: estimatedTimeToFailure
  type: string
- description: Model confidence in this prediction (0.0 to 1.0).
  name: confidenceScore
  type: number
- description: Recommended maintenance or operational action.
  name: recommendedAction
  type: string
- description: Timestamp when this prediction was generated.
  name: generatedAt
  type: string
provider_name: Baker Hughes
provider_slug: baker-hughes
schema_file: json-schema/baker-hughes-prediction-schema.json
slug: baker-hughes-prediction
source_filename: baker-hughes-prediction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/baker-hughes/json-schema/baker-hughes-prediction-schema.json\",\n  \"title\": \"Prediction\",\n  \"description\": \"AI-generated predictive maintenance forecast from Baker Hughes BHC3 AI Suite.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"predictionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the prediction.\"\n    },\n    \"assetId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the asset this prediction applies to.\"\n    },\n    \"predictionType\": {\n      \"type\": \"string\",\n      \"description\": \"Category of prediction.\",\n      \"enum\": [\"failure\", \"maintenance\", \"production\", \"efficiency\", \"well-integrity\"]\n    },\n    \"failureProbability\": {\n      \"type\": \"number\",\n      \"description\": \"Probability of failure in the next prediction window (0.0 to 1.0).\"\
  ,\n      \"minimum\": 0,\n      \"maximum\": 1\n    },\n    \"estimatedTimeToFailure\": {\n      \"type\": \"string\",\n      \"description\": \"Estimated time until failure expressed as ISO 8601 duration (e.g., P7D for 7 days).\"\n    },\n    \"confidenceScore\": {\n      \"type\": \"number\",\n      \"description\": \"Model confidence in this prediction (0.0 to 1.0).\",\n      \"minimum\": 0,\n      \"maximum\": 1\n    },\n    \"recommendedAction\": {\n      \"type\": \"string\",\n      \"description\": \"Recommended maintenance or operational action.\"\n    },\n    \"generatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when this prediction was generated.\"\n    }\n  },\n  \"required\": [\"predictionId\", \"assetId\", \"predictionType\", \"failureProbability\", \"recommendedAction\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/baker-hughes/refs/heads/main/json-schema/baker-hughes-prediction-schema.json
tags:
- Energy Technology
- Industrial IoT
- Oil And Gas
- Asset Performance Management
- Digital Energy
title: Prediction
---
