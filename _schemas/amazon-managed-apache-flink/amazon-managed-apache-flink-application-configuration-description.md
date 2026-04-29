---
description: Describes details about the application code and starting parameters for a Kinesis Data Analytics application.
layout: schema
name: ApplicationConfigurationDescription
properties_list:
- description: ''
  name: SqlApplicationConfigurationDescription
  type: object
- description: ''
  name: ApplicationCodeConfigurationDescription
  type: object
- description: ''
  name: RunConfigurationDescription
  type: object
- description: ''
  name: FlinkApplicationConfigurationDescription
  type: object
- description: ''
  name: EnvironmentPropertyDescriptions
  type: object
- description: ''
  name: ApplicationSnapshotConfigurationDescription
  type: object
- description: ''
  name: VpcConfigurationDescriptions
  type: object
- description: ''
  name: ZeppelinApplicationConfigurationDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-configuration-description-schema.json
slug: amazon-managed-apache-flink-application-configuration-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-configuration-description-schema.json\",\n  \"title\": \"ApplicationConfigurationDescription\",\n  \"description\": \"Describes details about the application code and starting parameters for a Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SqlApplicationConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SqlApplicationConfigurationDescription\"\n        },\n        {\n          \"description\": \"The details about inputs, outputs, and reference data sources for a SQL-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"ApplicationCodeConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationCodeConfigurationDescription\"\
  \n        },\n        {\n          \"description\": \"The details about the application code for a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"RunConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunConfigurationDescription\"\n        },\n        {\n          \"description\": \"The details about the starting properties for a Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"FlinkApplicationConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlinkApplicationConfigurationDescription\"\n        },\n        {\n          \"description\": \"The details about a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"EnvironmentPropertyDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentPropertyDescriptions\"\n        },\n        {\n          \"\
  description\": \"Describes execution properties for a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"ApplicationSnapshotConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationSnapshotConfigurationDescription\"\n        },\n        {\n          \"description\": \"Describes whether snapshots are enabled for a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"VpcConfigurationDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfigurationDescriptions\"\n        },\n        {\n          \"description\": \"The array of descriptions of VPC configurations available to the application.\"\n        }\n      ]\n    },\n    \"ZeppelinApplicationConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZeppelinApplicationConfigurationDescription\"\n        },\n        {\n    \
  \      \"description\": \"The configuration parameters for a Kinesis Data Analytics Studio notebook.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-configuration-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationConfigurationDescription
---
