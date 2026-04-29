---
description: Contains information about the column used to track time in a source data file.
layout: schema
name: TimestampColumn
properties_list:
- description: ''
  name: ColumnName
  type: object
- description: ''
  name: ColumnFormat
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-timestamp-column-schema.json
slug: amazon-lookout-for-metrics-timestamp-column
source_filename: amazon-lookout-for-metrics-timestamp-column-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-timestamp-column-schema.json\",\n  \"title\": \"TimestampColumn\",\n  \"description\": \"Contains information about the column used to track time in a source data file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ColumnName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnName\"\n        },\n        {\n          \"description\": \"The name of the timestamp column.\"\n        }\n      ]\n    },\n    \"ColumnFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeFormat\"\n        },\n        {\n          \"description\": \"The format of the timestamp column.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-timestamp-column-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: TimestampColumn
---
