---
description: A schema defining the structure and variables of events analyzed by Amazon Fraud Detector.
layout: schema
name: EventType
properties_list:
- description: Name of the event type.
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Variables included in each event of this type.
  name: eventVariables
  type: array
- description: Fraud/legit classification labels for this event type.
  name: labels
  type: array
- description: Entity types (e.g., customer, account) involved in this event.
  name: entityTypes
  type: array
- description: ''
  name: eventIngestion
  type: string
- description: ''
  name: arn
  type: string
provider_name: Amazon Fraud Detector
provider_slug: amazon-fraud-detector
schema_file: json-schema/amazon-fraud-detector-event-type-schema.json
slug: amazon-fraud-detector-event-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/json-schema/amazon-fraud-detector-event-type-schema.json\",\n  \"title\": \"EventType\",\n  \"description\": \"A schema defining the structure and variables of events analyzed by Amazon Fraud Detector.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the event type.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"eventVariables\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Variables included in each event of this type.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Fraud/legit classification labels for this event type.\"\n    },\n    \"\
  entityTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Entity types (e.g., customer, account) involved in this event.\"\n    },\n    \"eventIngestion\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ]\n    },\n    \"arn\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"eventVariables\",\n    \"labels\",\n    \"entityTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/json-schema/amazon-fraud-detector-event-type-schema.json
tags:
- AWS
- Financial Services
- Fraud Detection
- Machine Learning
- Security
title: EventType
---
