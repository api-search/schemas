---
description: A detected JSON format descriptor.
layout: schema
name: DetectedJsonFormatDescriptor
properties_list:
- description: ''
  name: FileCompression
  type: object
- description: ''
  name: Charset
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-detected-json-format-descriptor-schema.json
slug: amazon-lookout-for-metrics-detected-json-format-descriptor
source_filename: amazon-lookout-for-metrics-detected-json-format-descriptor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-json-format-descriptor-schema.json\",\n  \"title\": \"DetectedJsonFormatDescriptor\",\n  \"description\": \"A detected JSON format descriptor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileCompression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedField\"\n        },\n        {\n          \"description\": \"The format's file compression.\"\n        }\n      ]\n    },\n    \"Charset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedField\"\n        },\n        {\n          \"description\": \"The format's character set.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-json-format-descriptor-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DetectedJsonFormatDescriptor
---
