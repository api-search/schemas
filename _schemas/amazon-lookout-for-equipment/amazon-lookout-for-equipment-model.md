---
description: An Amazon Lookout for Equipment ML model for anomaly detection.
layout: schema
name: Model
properties_list:
- description: The name of the model.
  name: ModelName
  type: string
- description: The Amazon Resource Name (ARN) of the model.
  name: ModelArn
  type: string
- description: The name of the dataset used to train the model.
  name: DatasetName
  type: string
- description: The current status of the model.
  name: Status
  type: string
- description: Indicates the time reference in the dataset from which training data begins.
  name: TrainingDataStartTime
  type: string
- description: Indicates the time reference in the dataset from which training data ends.
  name: TrainingDataEndTime
  type: string
- description: The time at which the model was created.
  name: CreatedAt
  type: string
provider_name: Amazon Lookout for Equipment
provider_slug: amazon-lookout-for-equipment
schema_file: json-schema/amazon-lookout-for-equipment-model-schema.json
slug: amazon-lookout-for-equipment-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-equipment/refs/heads/main/json-schema/amazon-lookout-for-equipment-model-schema.json\",\n  \"title\": \"Model\",\n  \"description\": \"An Amazon Lookout for Equipment ML model for anomaly detection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModelName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the model.\",\n      \"example\": \"pump-failure-detector\"\n    },\n    \"ModelArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the model.\"\n    },\n    \"DatasetName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dataset used to train the model.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the model.\",\n      \"example\": \"SUCCESS\",\n      \"enum\": [\n\
  \        \"IN_PROGRESS\",\n        \"SUCCESS\",\n        \"FAILED\",\n        \"IMPORT_IN_PROGRESS\"\n      ]\n    },\n    \"TrainingDataStartTime\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the time reference in the dataset from which training data begins.\",\n      \"format\": \"date-time\"\n    },\n    \"TrainingDataEndTime\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the time reference in the dataset from which training data ends.\",\n      \"format\": \"date-time\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The time at which the model was created.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-equipment/refs/heads/main/json-schema/amazon-lookout-for-equipment-model-schema.json
tags:
- AWS
- Equipment Monitoring
- Industrial IoT
- Machine Learning
- Predictive Maintenance
title: Model
---
