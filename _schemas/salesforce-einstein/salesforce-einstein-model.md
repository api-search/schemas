---
description: Represents a trained machine learning model in Salesforce Einstein, used for image classification, object detection, text classification, or generative AI.
layout: schema
name: Einstein Model
properties_list:
- description: Unique model identifier.
  name: modelId
  type: string
- description: Display name of the model.
  name: name
  type: string
- description: ID of the dataset the model was trained on.
  name: datasetId
  type: integer
- description: Version of the dataset used for training.
  name: datasetVersionId
  type: integer
- description: Current status of the model.
  name: status
  type: string
- description: Training progress from 0.0 to 1.0.
  name: progress
  type: number
- description: Type of the model.
  name: modelType
  type: string
- description: Timestamp when the model was created.
  name: createdAt
  type: string
- description: Timestamp when the model was last updated.
  name: updatedAt
  type: string
- description: Number of training epochs.
  name: epochs
  type: integer
- description: Learning rate used during training.
  name: learningRate
  type: number
- description: Additional training parameters.
  name: trainParams
  type: object
- description: Training statistics and metrics.
  name: trainStats
  type: object
- description: Failure message if training failed.
  name: failureMsg
  type: string
- description: Object type identifier.
  name: object
  type: string
provider_name: Salesforce Einstein
provider_slug: salesforce-einstein
schema_file: json-schema/salesforce-einstein-model-schema.json
slug: salesforce-einstein-model
source_filename: salesforce-einstein-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/salesforce-einstein/json-schema/salesforce-einstein-model-schema.json\",\n  \"title\": \"Einstein Model\",\n  \"description\": \"Represents a trained machine learning model in Salesforce Einstein, used for image classification, object detection, text classification, or generative AI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"modelId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique model identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the model.\"\n    },\n    \"datasetId\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the dataset the model was trained on.\"\n    },\n    \"datasetVersionId\": {\n      \"type\": \"integer\",\n      \"description\": \"Version of the dataset used for training.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Current status of the model.\",\n      \"enum\": [\n        \"QUEUED\",\n        \"RUNNING\",\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"DELETED\"\n      ]\n    },\n    \"progress\": {\n      \"type\": \"number\",\n      \"description\": \"Training progress from 0.0 to 1.0.\",\n      \"minimum\": 0,\n      \"maximum\": 1\n    },\n    \"modelType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the model.\",\n      \"enum\": [\n        \"image\",\n        \"image-multi-label\",\n        \"image-detection\",\n        \"text-sentiment\",\n        \"text-intent\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the model was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the model was last updated.\"\n    },\n    \"epochs\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Number of training epochs.\",\n      \"minimum\": 1\n    },\n    \"learningRate\": {\n      \"type\": \"number\",\n      \"description\": \"Learning rate used during training.\",\n      \"exclusiveMinimum\": 0\n    },\n    \"trainParams\": {\n      \"type\": \"object\",\n      \"description\": \"Additional training parameters.\",\n      \"additionalProperties\": true\n    },\n    \"trainStats\": {\n      \"type\": \"object\",\n      \"description\": \"Training statistics and metrics.\",\n      \"properties\": {\n        \"labels\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of labels in the training data.\"\n        },\n        \"examples\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of training examples.\"\n        },\n        \"totalTime\": {\n          \"type\": \"string\",\n          \"description\": \"Total training time.\"\n        },\n        \"testAccuracy\": {\n          \"type\": \"number\"\
  ,\n          \"description\": \"Model accuracy on the test set.\"\n        },\n        \"trainingLoss\": {\n          \"type\": \"number\",\n          \"description\": \"Final training loss.\"\n        },\n        \"f1\": {\n          \"type\": \"number\",\n          \"description\": \"F1 score of the model.\"\n        }\n      }\n    },\n    \"failureMsg\": {\n      \"type\": \"string\",\n      \"description\": \"Failure message if training failed.\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"Object type identifier.\",\n      \"const\": \"model\"\n    }\n  },\n  \"required\": [\"modelId\", \"name\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/json-schema/salesforce-einstein-model-schema.json
tags:
- Artificial Intelligence
- Computer Vision
- CRM
- Machine Learning
- Natural Language Processing
- Predictive Analytics
- Salesforce
title: Einstein Model
---
