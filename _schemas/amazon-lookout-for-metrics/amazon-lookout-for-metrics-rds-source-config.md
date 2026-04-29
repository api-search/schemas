---
description: Contains information about the Amazon Relational Database Service (RDS) configuration.
layout: schema
name: RDSSourceConfig
properties_list:
- description: ''
  name: DBInstanceIdentifier
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
schema_file: json-schema/amazon-lookout-for-metrics-rds-source-config-schema.json
slug: amazon-lookout-for-metrics-rds-source-config
source_filename: amazon-lookout-for-metrics-rds-source-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-rds-source-config-schema.json\",\n  \"title\": \"RDSSourceConfig\",\n  \"description\": \"Contains information about the Amazon Relational Database Service (RDS) configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBInstanceIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RDSDatabaseIdentifier\"\n        },\n        {\n          \"description\": \"A string identifying the database instance.\"\n        }\n      ]\n    },\n    \"DatabaseHost\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseHost\"\n        },\n        {\n          \"description\": \"The host name of the database.\"\n        }\n      ]\n    },\n    \"DatabasePort\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/DatabasePort\"\n        },\n        {\n          \"description\": \"The port number where the database can be accessed.\"\n        }\n      ]\n    },\n    \"SecretManagerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoirotSecretManagerArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the AWS Secrets Manager role.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RDSDatabaseName\"\n        },\n        {\n          \"description\": \"The name of the RDS database.\"\n        }\n      ]\n    },\n    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TableName\"\n        },\n        {\n          \"description\": \"The name of the table in the database.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the role.\"\n        }\n      ]\n    },\n    \"VpcConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfiguration\"\n        },\n        {\n          \"description\": \"An object containing information about the Amazon Virtual Private Cloud (VPC) configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-rds-source-config-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: RDSSourceConfig
---
