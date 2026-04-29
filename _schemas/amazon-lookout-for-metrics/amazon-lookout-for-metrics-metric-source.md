---
description: Contains information about source data used to generate metrics.
layout: schema
name: MetricSource
properties_list:
- description: ''
  name: S3SourceConfig
  type: object
- description: ''
  name: AppFlowConfig
  type: object
- description: ''
  name: CloudWatchConfig
  type: object
- description: ''
  name: RDSSourceConfig
  type: object
- description: ''
  name: RedshiftSourceConfig
  type: object
- description: ''
  name: AthenaSourceConfig
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-metric-source-schema.json
slug: amazon-lookout-for-metrics-metric-source
source_filename: amazon-lookout-for-metrics-metric-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-source-schema.json\",\n  \"title\": \"MetricSource\",\n  \"description\": \"Contains information about source data used to generate metrics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3SourceConfig\": {\n      \"$ref\": \"#/components/schemas/S3SourceConfig\"\n    },\n    \"AppFlowConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AppFlowConfig\"\n        },\n        {\n          \"description\": \"Details about an AppFlow datasource.\"\n        }\n      ]\n    },\n    \"CloudWatchConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchConfig\"\n        },\n        {\n          \"description\": \"Details about an Amazon CloudWatch monitoring datasource.\"\n        }\n\
  \      ]\n    },\n    \"RDSSourceConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RDSSourceConfig\"\n        },\n        {\n          \"description\": \"Details about an Amazon Relational Database Service (RDS) datasource.\"\n        }\n      ]\n    },\n    \"RedshiftSourceConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RedshiftSourceConfig\"\n        },\n        {\n          \"description\": \"Details about an Amazon Redshift database datasource.\"\n        }\n      ]\n    },\n    \"AthenaSourceConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AthenaSourceConfig\"\n        },\n        {\n          \"description\": \"Details about an Amazon Athena datasource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-source-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: MetricSource
---
