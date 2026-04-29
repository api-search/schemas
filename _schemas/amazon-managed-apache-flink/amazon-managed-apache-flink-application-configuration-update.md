---
description: Describes updates to an application's configuration.
layout: schema
name: ApplicationConfigurationUpdate
properties_list:
- description: ''
  name: SqlApplicationConfigurationUpdate
  type: object
- description: ''
  name: ApplicationCodeConfigurationUpdate
  type: object
- description: ''
  name: FlinkApplicationConfigurationUpdate
  type: object
- description: ''
  name: EnvironmentPropertyUpdates
  type: object
- description: ''
  name: ApplicationSnapshotConfigurationUpdate
  type: object
- description: ''
  name: VpcConfigurationUpdates
  type: object
- description: ''
  name: ZeppelinApplicationConfigurationUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-configuration-update-schema.json
slug: amazon-managed-apache-flink-application-configuration-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-configuration-update-schema.json\",\n  \"title\": \"ApplicationConfigurationUpdate\",\n  \"description\": \"Describes updates to an application's configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SqlApplicationConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SqlApplicationConfigurationUpdate\"\n        },\n        {\n          \"description\": \"Describes updates to a SQL-based Kinesis Data Analytics application's configuration.\"\n        }\n      ]\n    },\n    \"ApplicationCodeConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationCodeConfigurationUpdate\"\n        },\n        {\n          \"description\": \"Describes updates\
  \ to an application's code configuration.\"\n        }\n      ]\n    },\n    \"FlinkApplicationConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlinkApplicationConfigurationUpdate\"\n        },\n        {\n          \"description\": \"Describes updates to a Flink-based Kinesis Data Analytics application's configuration.\"\n        }\n      ]\n    },\n    \"EnvironmentPropertyUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentPropertyUpdates\"\n        },\n        {\n          \"description\": \"Describes updates to the environment properties for a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"ApplicationSnapshotConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationSnapshotConfigurationUpdate\"\n        },\n        {\n          \"description\": \"Describes whether snapshots are enabled for a Flink-based\
  \ Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"VpcConfigurationUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfigurationUpdates\"\n        },\n        {\n          \"description\": \"Updates to the array of descriptions of VPC configurations available to the application.\"\n        }\n      ]\n    },\n    \"ZeppelinApplicationConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZeppelinApplicationConfigurationUpdate\"\n        },\n        {\n          \"description\": \"Updates to the configuration of a Kinesis Data Analytics Studio notebook.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-configuration-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationConfigurationUpdate
---
