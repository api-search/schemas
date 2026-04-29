---
description: Properties of an inferred data format.
layout: schema
name: DetectedFileFormatDescriptor
properties_list:
- description: ''
  name: CsvFormatDescriptor
  type: object
- description: ''
  name: JsonFormatDescriptor
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-detected-file-format-descriptor-schema.json
slug: amazon-lookout-for-metrics-detected-file-format-descriptor
source_filename: amazon-lookout-for-metrics-detected-file-format-descriptor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-file-format-descriptor-schema.json\",\n  \"title\": \"DetectedFileFormatDescriptor\",\n  \"description\": \"Properties of an inferred data format.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CsvFormatDescriptor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedCsvFormatDescriptor\"\n        },\n        {\n          \"description\": \"Details about a CSV format.\"\n        }\n      ]\n    },\n    \"JsonFormatDescriptor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedJsonFormatDescriptor\"\n        },\n        {\n          \"description\": \"Details about a JSON format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-file-format-descriptor-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DetectedFileFormatDescriptor
---
