---
description: A logical grouping of Amazon Forecast datasets for training a predictor.
layout: schema
name: DatasetGroup
properties_list:
- description: ARN of the dataset group.
  name: DatasetGroupArn
  type: string
- description: Name of the dataset group.
  name: DatasetGroupName
  type: string
- description: Domain of the dataset group.
  name: Domain
  type: string
- description: ARNs of datasets in this group.
  name: DatasetArns
  type: array
- description: ''
  name: Status
  type: string
- description: ''
  name: CreationTime
  type: string
- description: ''
  name: LastModificationTime
  type: string
provider_name: Amazon Forecast
provider_slug: amazon-forecast
schema_file: json-schema/amazon-forecast-dataset-group-schema.json
slug: amazon-forecast-dataset-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-forecast/refs/heads/main/json-schema/amazon-forecast-dataset-group-schema.json\",\n  \"title\": \"DatasetGroup\",\n  \"description\": \"A logical grouping of Amazon Forecast datasets for training a predictor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetGroupArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the dataset group.\"\n    },\n    \"DatasetGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the dataset group.\"\n    },\n    \"Domain\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"RETAIL\",\n        \"CUSTOM\",\n        \"INVENTORY_PLANNING\",\n        \"EC2_CAPACITY\",\n        \"WORK_FORCE\",\n        \"WEB_TRAFFIC\",\n        \"METRICS\"\n      ],\n      \"description\": \"Domain of the dataset group.\"\n    },\n    \"DatasetArns\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"ARNs of datasets in this group.\"\n    },\n    \"Status\": {\n      \"type\": \"string\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"LastModificationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"DatasetGroupName\",\n    \"Domain\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-forecast/refs/heads/main/json-schema/amazon-forecast-dataset-group-schema.json
tags:
- AWS
- Forecasting
- Machine Learning
- Predictive Analytics
- Time Series
title: DatasetGroup
---
