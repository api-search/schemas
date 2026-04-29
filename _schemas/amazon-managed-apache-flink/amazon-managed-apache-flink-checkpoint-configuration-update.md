---
description: Describes updates to the checkpointing parameters for a Flink-based Kinesis Data Analytics application.
layout: schema
name: CheckpointConfigurationUpdate
properties_list:
- description: ''
  name: ConfigurationTypeUpdate
  type: object
- description: ''
  name: CheckpointingEnabledUpdate
  type: object
- description: ''
  name: CheckpointIntervalUpdate
  type: object
- description: ''
  name: MinPauseBetweenCheckpointsUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-checkpoint-configuration-update-schema.json
slug: amazon-managed-apache-flink-checkpoint-configuration-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-checkpoint-configuration-update-schema.json\",\n  \"title\": \"CheckpointConfigurationUpdate\",\n  \"description\": \"Describes updates to the checkpointing parameters for a Flink-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationTypeUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationType\"\n        },\n        {\n          \"description\": \"<p>Describes updates to whether the application uses the default checkpointing behavior of Kinesis Data Analytics. You must set this property to <code>CUSTOM</code> in order to set the <code>CheckpointingEnabled</code>, <code>CheckpointInterval</code>, or <code>MinPauseBetweenCheckpoints</code> parameters. </p> <note>\
  \ <p>If this value is set to <code>DEFAULT</code>, the application will use the following values, even if they are set to other values using APIs or application code:</p> <ul> <li> <p> <b>CheckpointingEnabled:</b> true</p> </li> <li> <p> <b>CheckpointInterval:</b> 60000</p> </li> <li> <p> <b>MinPauseBetweenCheckpoints:</b> 5000</p> </li> </ul> </note>\"\n        }\n      ]\n    },\n    \"CheckpointingEnabledUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"<p>Describes updates to whether checkpointing is enabled for an application.</p> <note> <p>If <code>CheckpointConfiguration.ConfigurationType</code> is <code>DEFAULT</code>, the application will use a <code>CheckpointingEnabled</code> value of <code>true</code>, even if this value is set to another value using this API or in application code.</p> </note>\"\n        }\n      ]\n    },\n    \"CheckpointIntervalUpdate\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckpointInterval\"\n        },\n        {\n          \"description\": \"<p>Describes updates to the interval in milliseconds between checkpoint operations.</p> <note> <p>If <code>CheckpointConfiguration.ConfigurationType</code> is <code>DEFAULT</code>, the application will use a <code>CheckpointInterval</code> value of 60000, even if this value is set to another value using this API or in application code.</p> </note>\"\n        }\n      ]\n    },\n    \"MinPauseBetweenCheckpointsUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinPauseBetweenCheckpoints\"\n        },\n        {\n          \"description\": \"<p>Describes updates to the minimum time in milliseconds after a checkpoint operation completes that a new checkpoint operation can start.</p> <note> <p>If <code>CheckpointConfiguration.ConfigurationType</code> is <code>DEFAULT</code>, the application will use a <code>MinPauseBetweenCheckpoints</code>\
  \ value of 5000, even if this value is set using this API or in application code.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-checkpoint-configuration-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CheckpointConfigurationUpdate
---
