---
description: An Amazon Forecast dataset containing time-series training data.
layout: schema
name: Dataset
properties_list:
- description: ARN of the dataset.
  name: DatasetArn
  type: string
- description: Name of the dataset.
  name: DatasetName
  type: string
- description: Domain for the dataset.
  name: Domain
  type: string
- description: Type of the dataset.
  name: DatasetType
  type: string
- description: Frequency of data points (e.g., D for daily, H for hourly).
  name: DataFrequency
  type: string
- description: Status of the dataset.
  name: Status
  type: string
- description: Time the dataset was created.
  name: CreationTime
  type: string
- description: Time the dataset was last modified.
  name: LastModificationTime
  type: string
provider_name: Amazon Forecast
provider_slug: amazon-forecast
schema_file: json-schema/amazon-forecast-dataset-schema.json
slug: amazon-forecast-dataset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-forecast/refs/heads/main/json-schema/amazon-forecast-dataset-schema.json\",\n  \"title\": \"Dataset\",\n  \"description\": \"An Amazon Forecast dataset containing time-series training data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the dataset.\"\n    },\n    \"DatasetName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the dataset.\"\n    },\n    \"Domain\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"RETAIL\",\n        \"CUSTOM\",\n        \"INVENTORY_PLANNING\",\n        \"EC2_CAPACITY\",\n        \"WORK_FORCE\",\n        \"WEB_TRAFFIC\",\n        \"METRICS\"\n      ],\n      \"description\": \"Domain for the dataset.\"\n    },\n    \"DatasetType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"\
  TARGET_TIME_SERIES\",\n        \"RELATED_TIME_SERIES\",\n        \"ITEM_METADATA\"\n      ],\n      \"description\": \"Type of the dataset.\"\n    },\n    \"DataFrequency\": {\n      \"type\": \"string\",\n      \"description\": \"Frequency of data points (e.g., D for daily, H for hourly).\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the dataset.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time the dataset was created.\"\n    },\n    \"LastModificationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time the dataset was last modified.\"\n    }\n  },\n  \"required\": [\n    \"DatasetName\",\n    \"Domain\",\n    \"DatasetType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-forecast/refs/heads/main/json-schema/amazon-forecast-dataset-schema.json
tags:
- AWS
- Forecasting
- Machine Learning
- Predictive Analytics
- Time Series
title: Dataset
---
