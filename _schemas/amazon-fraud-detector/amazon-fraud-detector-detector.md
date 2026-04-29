---
description: An Amazon Fraud Detector that orchestrates ML models and business rules for real-time fraud decisions.
layout: schema
name: Detector
properties_list:
- description: Unique identifier for the detector.
  name: detectorId
  type: string
- description: Optional description of the detector.
  name: description
  type: string
- description: The name of the event type associated with the detector.
  name: eventTypeName
  type: string
- description: ''
  name: lastUpdatedTime
  type: string
- description: ''
  name: createdTime
  type: string
- description: ARN of the detector.
  name: arn
  type: string
provider_name: Amazon Fraud Detector
provider_slug: amazon-fraud-detector
schema_file: json-schema/amazon-fraud-detector-detector-schema.json
slug: amazon-fraud-detector-detector
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/json-schema/amazon-fraud-detector-detector-schema.json\",\n  \"title\": \"Detector\",\n  \"description\": \"An Amazon Fraud Detector that orchestrates ML models and business rules for real-time fraud decisions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the detector.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the detector.\"\n    },\n    \"eventTypeName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the event type associated with the detector.\"\n    },\n    \"lastUpdatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"\
  format\": \"date-time\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the detector.\"\n    }\n  },\n  \"required\": [\n    \"detectorId\",\n    \"eventTypeName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/json-schema/amazon-fraud-detector-detector-schema.json
tags:
- AWS
- Financial Services
- Fraud Detection
- Machine Learning
- Security
title: Detector
---
