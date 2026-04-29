---
description: Contains information about the source configuration in Amazon S3.
layout: schema
name: SampleDataS3SourceConfig
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
schema_file: json-schema/amazon-lookout-for-metrics-sample-data-s3-source-config-schema.json
slug: amazon-lookout-for-metrics-sample-data-s3-source-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-sample-data-s3-source-config-schema.json\",\n  \"title\": \"SampleDataS3SourceConfig\",\n  \"description\": \"Contains information about the source configuration in Amazon S3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the role.\"\n        }\n      ]\n    },\n    \"TemplatedPathList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplatedPathList\"\n        },\n        {\n          \"description\": \"An array of strings containing the list of templated paths.\"\n        }\n      ]\n    },\n    \"HistoricalDataPathList\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/HistoricalDataPathList\"\n        },\n        {\n          \"description\": \"An array of strings containing the historical set of data paths.\"\n        }\n      ]\n    },\n    \"FileFormatDescriptor\": {\n      \"$ref\": \"#/components/schemas/FileFormatDescriptor\"\n    }\n  },\n  \"required\": [\n    \"RoleArn\",\n    \"FileFormatDescriptor\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-sample-data-s3-source-config-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: SampleDataS3SourceConfig
---
