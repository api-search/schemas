---
description: An Amazon Fraud Detector ML model trained to score transactions for fraud risk.
layout: schema
name: Model
properties_list:
- description: Unique identifier for the model.
  name: modelId
  type: string
- description: The type of fraud detection model.
  name: modelType
  type: string
- description: ''
  name: description
  type: string
- description: The event type used to train and score.
  name: eventTypeName
  type: string
- description: ''
  name: arn
  type: string
- description: ''
  name: lastUpdatedTime
  type: string
- description: ''
  name: createdTime
  type: string
provider_name: Amazon Fraud Detector
provider_slug: amazon-fraud-detector
schema_file: json-schema/amazon-fraud-detector-model-schema.json
slug: amazon-fraud-detector-model
source_filename: amazon-fraud-detector-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/json-schema/amazon-fraud-detector-model-schema.json\",\n  \"title\": \"Model\",\n  \"description\": \"An Amazon Fraud Detector ML model trained to score transactions for fraud risk.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"modelId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the model.\"\n    },\n    \"modelType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ONLINE_FRAUD_INSIGHTS\",\n        \"TRANSACTION_FRAUD_INSIGHTS\",\n        \"ACCOUNT_TAKEOVER_INSIGHTS\"\n      ],\n      \"description\": \"The type of fraud detection model.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"eventTypeName\": {\n      \"type\": \"string\",\n      \"description\": \"The event type used to train and score.\"\n    },\n    \"arn\"\
  : {\n      \"type\": \"string\"\n    },\n    \"lastUpdatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"modelId\",\n    \"modelType\",\n    \"eventTypeName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/json-schema/amazon-fraud-detector-model-schema.json
tags:
- Financial Services
- Fraud Detection
- Machine Learning
- Security
title: Model
---
