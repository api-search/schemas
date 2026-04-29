---
description: Describes configuration parameters for a Flink-based Kinesis Data Analytics application or a Studio notebook.
layout: schema
name: FlinkApplicationConfiguration
properties_list:
- description: ''
  name: CheckpointConfiguration
  type: object
- description: ''
  name: MonitoringConfiguration
  type: object
- description: ''
  name: ParallelismConfiguration
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-flink-application-configuration-schema.json
slug: amazon-managed-apache-flink-flink-application-configuration
source_filename: amazon-managed-apache-flink-flink-application-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-flink-application-configuration-schema.json\",\n  \"title\": \"FlinkApplicationConfiguration\",\n  \"description\": \"Describes configuration parameters for a Flink-based Kinesis Data Analytics application or a Studio notebook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CheckpointConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckpointConfiguration\"\n        },\n        {\n          \"description\": \"Describes an application's checkpointing configuration. Checkpointing is the process of persisting application state for fault tolerance. For more information, see <a href=\\\"https://ci.apache.org/projects/flink/flink-docs-release-1.8/concepts/programming-model.html#checkpoints-for-fault-tolerance\\\"> Checkpoints\
  \ for Fault Tolerance</a> in the <a href=\\\"https://ci.apache.org/projects/flink/flink-docs-release-1.8/\\\">Apache Flink Documentation</a>. \"\n        }\n      ]\n    },\n    \"MonitoringConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MonitoringConfiguration\"\n        },\n        {\n          \"description\": \"Describes configuration parameters for Amazon CloudWatch logging for an application.\"\n        }\n      ]\n    },\n    \"ParallelismConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParallelismConfiguration\"\n        },\n        {\n          \"description\": \"Describes parameters for how an application executes multiple tasks simultaneously.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-flink-application-configuration-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: FlinkApplicationConfiguration
---
