---
description: Provides information about the Amazon Redshift database configuration.
layout: schema
name: RedshiftSourceConfig
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: DatabaseHost
  type: object
- description: ''
  name: DatabasePort
  type: object
- description: ''
  name: SecretManagerArn
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: TableName
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: VpcConfiguration
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-redshift-source-config-schema.json
slug: amazon-lookout-for-metrics-redshift-source-config
source_filename: amazon-lookout-for-metrics-redshift-source-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-redshift-source-config-schema.json\",\n  \"title\": \"RedshiftSourceConfig\",\n  \"description\": \"Provides information about the Amazon Redshift database configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RedshiftClusterIdentifier\"\n        },\n        {\n          \"description\": \"A string identifying the Redshift cluster.\"\n        }\n      ]\n    },\n    \"DatabaseHost\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseHost\"\n        },\n        {\n          \"description\": \"The name of the database host.\"\n        }\n      ]\n    },\n    \"DatabasePort\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/DatabasePort\"\n        },\n        {\n          \"description\": \"The port number where the database can be accessed.\"\n        }\n      ]\n    },\n    \"SecretManagerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoirotSecretManagerArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the AWS Secrets Manager role.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RedshiftDatabaseName\"\n        },\n        {\n          \"description\": \"The Redshift database name.\"\n        }\n      ]\n    },\n    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TableName\"\n        },\n        {\n          \"description\": \"The table name of the Redshift database.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the role providing access to the database.\"\n        }\n      ]\n    },\n    \"VpcConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfiguration\"\n        },\n        {\n          \"description\": \"Contains information about the Amazon Virtual Private Cloud (VPC) configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-redshift-source-config-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: RedshiftSourceConfig
---
