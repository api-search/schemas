---
description: Describes an application's checkpointing configuration. Checkpointing is the process of persisting application state for fault tolerance. For more information, see <a href="https://ci.apache.org/projects/flink/flink-docs-release-1.8/concepts/programming-model.html#checkpoints-for-fault-tolerance"> Checkpoints for Fault Tolerance</a> in the <a href="https://ci.apache.org/projects/flink/flink-docs-release-1.8/">Apache Flink Documentation</a>.
layout: schema
name: CheckpointConfiguration
properties_list:
- description: ''
  name: ConfigurationType
  type: object
- description: ''
  name: CheckpointingEnabled
  type: object
- description: ''
  name: CheckpointInterval
  type: object
- description: ''
  name: MinPauseBetweenCheckpoints
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-checkpoint-configuration-schema.json
slug: amazon-managed-apache-flink-checkpoint-configuration
source_filename: amazon-managed-apache-flink-checkpoint-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-checkpoint-configuration-schema.json\",\n  \"title\": \"CheckpointConfiguration\",\n  \"description\": \"Describes an application's checkpointing configuration. Checkpointing is the process of persisting application state for fault tolerance. For more information, see <a href=\\\"https://ci.apache.org/projects/flink/flink-docs-release-1.8/concepts/programming-model.html#checkpoints-for-fault-tolerance\\\"> Checkpoints for Fault Tolerance</a> in the <a href=\\\"https://ci.apache.org/projects/flink/flink-docs-release-1.8/\\\">Apache Flink Documentation</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationType\"\n        },\n        {\n          \"\
  description\": \"<p>Describes whether the application uses Kinesis Data Analytics' default checkpointing behavior. You must set this property to <code>CUSTOM</code> in order to set the <code>CheckpointingEnabled</code>, <code>CheckpointInterval</code>, or <code>MinPauseBetweenCheckpoints</code> parameters.</p> <note> <p>If this value is set to <code>DEFAULT</code>, the application will use the following values, even if they are set to other values using APIs or application code:</p> <ul> <li> <p> <b>CheckpointingEnabled:</b> true</p> </li> <li> <p> <b>CheckpointInterval:</b> 60000</p> </li> <li> <p> <b>MinPauseBetweenCheckpoints:</b> 5000</p> </li> </ul> </note>\"\n        }\n      ]\n    },\n    \"CheckpointingEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"<p>Describes whether checkpointing is enabled for a Flink-based Kinesis Data Analytics application.</p> <note> <p>If <code>CheckpointConfiguration.ConfigurationType</code>\
  \ is <code>DEFAULT</code>, the application will use a <code>CheckpointingEnabled</code> value of <code>true</code>, even if this value is set to another value using this API or in application code.</p> </note>\"\n        }\n      ]\n    },\n    \"CheckpointInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckpointInterval\"\n        },\n        {\n          \"description\": \"<p>Describes the interval in milliseconds between checkpoint operations. </p> <note> <p>If <code>CheckpointConfiguration.ConfigurationType</code> is <code>DEFAULT</code>, the application will use a <code>CheckpointInterval</code> value of 60000, even if this value is set to another value using this API or in application code.</p> </note>\"\n        }\n      ]\n    },\n    \"MinPauseBetweenCheckpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinPauseBetweenCheckpoints\"\n        },\n        {\n          \"description\": \"<p>Describes the\
  \ minimum time in milliseconds after a checkpoint operation completes that a new checkpoint operation can start. If a checkpoint operation takes longer than the <code>CheckpointInterval</code>, the application otherwise performs continual checkpoint operations. For more information, see <a href=\\\"https://ci.apache.org/projects/flink/flink-docs-release-1.8/ops/state/large_state_tuning.html#tuning-checkpointing\\\"> Tuning Checkpointing</a> in the <a href=\\\"https://ci.apache.org/projects/flink/flink-docs-release-1.8/\\\">Apache Flink Documentation</a>.</p> <note> <p>If <code>CheckpointConfiguration.ConfigurationType</code> is <code>DEFAULT</code>, the application will use a <code>MinPauseBetweenCheckpoints</code> value of 5000, even if this value is set using this API or in application code.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-checkpoint-configuration-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CheckpointConfiguration
---
