---
description: Specifies the creation parameters for a Kinesis Data Analytics application.
layout: schema
name: ApplicationConfiguration
properties_list:
- description: ''
  name: SqlApplicationConfiguration
  type: object
- description: ''
  name: FlinkApplicationConfiguration
  type: object
- description: ''
  name: EnvironmentProperties
  type: object
- description: ''
  name: ApplicationCodeConfiguration
  type: object
- description: ''
  name: ApplicationSnapshotConfiguration
  type: object
- description: ''
  name: VpcConfigurations
  type: object
- description: ''
  name: ZeppelinApplicationConfiguration
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-configuration-schema.json
slug: amazon-managed-apache-flink-application-configuration
source_filename: amazon-managed-apache-flink-application-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-configuration-schema.json\",\n  \"title\": \"ApplicationConfiguration\",\n  \"description\": \"Specifies the creation parameters for a Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SqlApplicationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SqlApplicationConfiguration\"\n        },\n        {\n          \"description\": \"The creation and update parameters for a SQL-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"FlinkApplicationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlinkApplicationConfiguration\"\n        },\n        {\n          \"description\": \"The creation and update\
  \ parameters for a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"EnvironmentProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentProperties\"\n        },\n        {\n          \"description\": \"Describes execution properties for a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"ApplicationCodeConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationCodeConfiguration\"\n        },\n        {\n          \"description\": \"The code location and type parameters for a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"ApplicationSnapshotConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationSnapshotConfiguration\"\n        },\n        {\n          \"description\": \"Describes whether snapshots are enabled for a Flink-based Kinesis Data Analytics\
  \ application.\"\n        }\n      ]\n    },\n    \"VpcConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfigurations\"\n        },\n        {\n          \"description\": \"The array of descriptions of VPC configurations available to the application.\"\n        }\n      ]\n    },\n    \"ZeppelinApplicationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZeppelinApplicationConfiguration\"\n        },\n        {\n          \"description\": \"The configuration parameters for a Kinesis Data Analytics Studio notebook.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-configuration-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationConfiguration
---
