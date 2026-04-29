---
description: Describes updates to whether snapshots are enabled for a Flink-based Kinesis Data Analytics application.
layout: schema
name: ApplicationSnapshotConfigurationUpdate
properties_list:
- description: ''
  name: SnapshotsEnabledUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-snapshot-configuration-update-schema.json
slug: amazon-managed-apache-flink-application-snapshot-configuration-update
source_filename: amazon-managed-apache-flink-application-snapshot-configuration-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-snapshot-configuration-update-schema.json\",\n  \"title\": \"ApplicationSnapshotConfigurationUpdate\",\n  \"description\": \"Describes updates to whether snapshots are enabled for a Flink-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotsEnabledUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Describes updates to whether snapshots are enabled for an application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SnapshotsEnabledUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-snapshot-configuration-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationSnapshotConfigurationUpdate
---
