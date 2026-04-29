---
description: An Amazon Lookout for Equipment dataset containing equipment sensor data.
layout: schema
name: Dataset
properties_list:
- description: The name of the dataset.
  name: DatasetName
  type: string
- description: The Amazon Resource Name (ARN) of the dataset.
  name: DatasetArn
  type: string
- description: The current status of the dataset.
  name: Status
  type: string
- description: The time at which the dataset was created.
  name: CreatedAt
  type: string
- description: The time at which the dataset was last updated.
  name: LastUpdatedAt
  type: string
provider_name: Amazon Lookout for Equipment
provider_slug: amazon-lookout-for-equipment
schema_file: json-schema/amazon-lookout-for-equipment-dataset-schema.json
slug: amazon-lookout-for-equipment-dataset
source_filename: amazon-lookout-for-equipment-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-equipment/refs/heads/main/json-schema/amazon-lookout-for-equipment-dataset-schema.json\",\n  \"title\": \"Dataset\",\n  \"description\": \"An Amazon Lookout for Equipment dataset containing equipment sensor data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dataset.\",\n      \"example\": \"pump-sensors-dataset\"\n    },\n    \"DatasetArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the dataset.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the dataset.\",\n      \"example\": \"ACTIVE\",\n      \"enum\": [\n        \"CREATED\",\n        \"INGESTION_IN_PROGRESS\",\n        \"ACTIVE\"\n      ]\n    },\n    \"CreatedAt\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The time at which the dataset was created.\",\n      \"format\": \"date-time\"\n    },\n    \"LastUpdatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The time at which the dataset was last updated.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-equipment/refs/heads/main/json-schema/amazon-lookout-for-equipment-dataset-schema.json
tags:
- AWS
- Equipment Monitoring
- Industrial IoT
- Machine Learning
- Predictive Maintenance
title: Dataset
---
