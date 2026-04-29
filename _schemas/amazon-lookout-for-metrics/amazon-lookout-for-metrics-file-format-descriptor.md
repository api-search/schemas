---
description: Contains information about a source file's formatting.
layout: schema
name: FileFormatDescriptor
properties_list:
- description: ''
  name: CsvFormatDescriptor
  type: object
- description: ''
  name: JsonFormatDescriptor
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-file-format-descriptor-schema.json
slug: amazon-lookout-for-metrics-file-format-descriptor
source_filename: amazon-lookout-for-metrics-file-format-descriptor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-file-format-descriptor-schema.json\",\n  \"title\": \"FileFormatDescriptor\",\n  \"description\": \"Contains information about a source file's formatting.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CsvFormatDescriptor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CsvFormatDescriptor\"\n        },\n        {\n          \"description\": \"Contains information about how a source CSV data file should be analyzed.\"\n        }\n      ]\n    },\n    \"JsonFormatDescriptor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JsonFormatDescriptor\"\n        },\n        {\n          \"description\": \"Contains information about how a source JSON data file should be analyzed.\"\n        }\n      ]\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-file-format-descriptor-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: FileFormatDescriptor
---
