---
description: Details about an Amazon Athena datasource.
layout: schema
name: AthenaSourceConfig
properties_list:
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: DataCatalog
  type: object
- description: ''
  name: TableName
  type: object
- description: ''
  name: WorkGroupName
  type: object
- description: ''
  name: S3ResultsPath
  type: object
- description: ''
  name: BackTestConfiguration
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-athena-source-config-schema.json
slug: amazon-lookout-for-metrics-athena-source-config
source_filename: amazon-lookout-for-metrics-athena-source-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-athena-source-config-schema.json\",\n  \"title\": \"AthenaSourceConfig\",\n  \"description\": \"Details about an Amazon Athena datasource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"An IAM role that gives Amazon Lookout for Metrics permission to access the data.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AthenaDatabaseName\"\n        },\n        {\n          \"description\": \"The database's name.\"\n        }\n      ]\n    },\n    \"DataCatalog\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AthenaDataCatalog\"\
  \n        },\n        {\n          \"description\": \"The database's data catalog.\"\n        }\n      ]\n    },\n    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AthenaTableName\"\n        },\n        {\n          \"description\": \"The database's table name.\"\n        }\n      ]\n    },\n    \"WorkGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AthenaWorkGroupName\"\n        },\n        {\n          \"description\": \"The database's work group name.\"\n        }\n      ]\n    },\n    \"S3ResultsPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AthenaS3ResultsPath\"\n        },\n        {\n          \"description\": \"The database's results path.\"\n        }\n      ]\n    },\n    \"BackTestConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BackTestConfiguration\"\n        },\n        {\n          \"description\": \"Settings\
  \ for backtest mode.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-athena-source-config-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AthenaSourceConfig
---
