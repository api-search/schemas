---
description: Describes updates to the configuration parameters for a Flink-based Kinesis Data Analytics application.
layout: schema
name: FlinkApplicationConfigurationUpdate
properties_list:
- description: ''
  name: CheckpointConfigurationUpdate
  type: object
- description: ''
  name: MonitoringConfigurationUpdate
  type: object
- description: ''
  name: ParallelismConfigurationUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-flink-application-configuration-update-schema.json
slug: amazon-managed-apache-flink-flink-application-configuration-update
source_filename: amazon-managed-apache-flink-flink-application-configuration-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-flink-application-configuration-update-schema.json\",\n  \"title\": \"FlinkApplicationConfigurationUpdate\",\n  \"description\": \"Describes updates to the configuration parameters for a Flink-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CheckpointConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckpointConfigurationUpdate\"\n        },\n        {\n          \"description\": \"Describes updates to an application's checkpointing configuration. Checkpointing is the process of persisting application state for fault tolerance.\"\n        }\n      ]\n    },\n    \"MonitoringConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MonitoringConfigurationUpdate\"\
  \n        },\n        {\n          \"description\": \"Describes updates to the configuration parameters for Amazon CloudWatch logging for an application.\"\n        }\n      ]\n    },\n    \"ParallelismConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParallelismConfigurationUpdate\"\n        },\n        {\n          \"description\": \"Describes updates to the parameters for how an application executes multiple tasks simultaneously.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-flink-application-configuration-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: FlinkApplicationConfigurationUpdate
---
