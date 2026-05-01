---
description: Contains information about the configuration of the S3 bucket that contains source files.
layout: schema
name: S3SourceConfig
properties_list:
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: TemplatedPathList
  type: object
- description: ''
  name: HistoricalDataPathList
  type: object
- description: ''
  name: FileFormatDescriptor
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-s3-source-config-schema.json
slug: amazon-lookout-for-metrics-s3-source-config
source_filename: amazon-lookout-for-metrics-s3-source-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-s3-source-config-schema.json\",\n  \"title\": \"S3SourceConfig\",\n  \"description\": \"Contains information about the configuration of the S3 bucket that contains source files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of an IAM role that has read and write access permissions to the source S3 bucket.\"\n        }\n      ]\n    },\n    \"TemplatedPathList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplatedPathList\"\n        },\n        {\n          \"description\": \"A list of templated paths to the source files.\"\n        }\n      ]\n    },\n    \"HistoricalDataPathList\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HistoricalDataPathList\"\n        },\n        {\n          \"description\": \"A list of paths to the historical data files.\"\n        }\n      ]\n    },\n    \"FileFormatDescriptor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileFormatDescriptor\"\n        },\n        {\n          \"description\": \"Contains information about a source file's formatting.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-s3-source-config-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: S3SourceConfig
---
