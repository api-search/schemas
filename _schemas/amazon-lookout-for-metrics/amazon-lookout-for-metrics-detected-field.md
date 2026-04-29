---
description: An inferred field.
layout: schema
name: DetectedField
properties_list:
- description: ''
  name: Value
  type: object
- description: ''
  name: Confidence
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-detected-field-schema.json
slug: amazon-lookout-for-metrics-detected-field
source_filename: amazon-lookout-for-metrics-detected-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-field-schema.json\",\n  \"title\": \"DetectedField\",\n  \"description\": \"An inferred field.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeValue\"\n        },\n        {\n          \"description\": \"The field's value.\"\n        }\n      ]\n    },\n    \"Confidence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Confidence\"\n        },\n        {\n          \"description\": \"The field's confidence.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The field's message.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-field-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DetectedField
---
