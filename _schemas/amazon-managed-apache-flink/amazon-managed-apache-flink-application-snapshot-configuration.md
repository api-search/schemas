---
description: Describes whether snapshots are enabled for a Flink-based Kinesis Data Analytics application.
layout: schema
name: ApplicationSnapshotConfiguration
properties_list:
- description: ''
  name: SnapshotsEnabled
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-snapshot-configuration-schema.json
slug: amazon-managed-apache-flink-application-snapshot-configuration
source_filename: amazon-managed-apache-flink-application-snapshot-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-snapshot-configuration-schema.json\",\n  \"title\": \"ApplicationSnapshotConfiguration\",\n  \"description\": \"Describes whether snapshots are enabled for a Flink-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotsEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Describes whether snapshots are enabled for a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SnapshotsEnabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-snapshot-configuration-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationSnapshotConfiguration
---
