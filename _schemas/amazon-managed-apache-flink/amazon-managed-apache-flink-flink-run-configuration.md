---
description: Describes the starting parameters for a Flink-based Kinesis Data Analytics application.
layout: schema
name: FlinkRunConfiguration
properties_list:
- description: ''
  name: AllowNonRestoredState
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-flink-run-configuration-schema.json
slug: amazon-managed-apache-flink-flink-run-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-flink-run-configuration-schema.json\",\n  \"title\": \"FlinkRunConfiguration\",\n  \"description\": \"Describes the starting parameters for a Flink-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AllowNonRestoredState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"<p>When restoring from a snapshot, specifies whether the runtime is allowed to skip a state that cannot be mapped to the new program. This will happen if the program is updated between snapshots to remove stateful parameters, and state data in the snapshot no longer corresponds to valid application data. For more information, see <a href=\\\"https://ci.apache.org/projects/flink/flink-docs-release-1.8/ops/state/savepoints.html#allowing-non-restored-state\\\
  \"> Allowing Non-Restored State</a> in the <a href=\\\"https://ci.apache.org/projects/flink/flink-docs-release-1.8/\\\">Apache Flink documentation</a>.</p> <note> <p>This value defaults to <code>false</code>. If you update your application without specifying this parameter, <code>AllowNonRestoredState</code> will be set to <code>false</code>, even if it was previously set to <code>true</code>.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-flink-run-configuration-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: FlinkRunConfiguration
---
