---
description: Describes whether snapshots are enabled for a Flink-based Kinesis Data Analytics application.
layout: schema
name: ApplicationSnapshotConfigurationDescription
properties_list:
- description: ''
  name: SnapshotsEnabled
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-snapshot-configuration-description-schema.json
slug: amazon-managed-apache-flink-application-snapshot-configuration-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-snapshot-configuration-description-schema.json\",\n  \"title\": \"ApplicationSnapshotConfigurationDescription\",\n  \"description\": \"Describes whether snapshots are enabled for a Flink-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotsEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Describes whether snapshots are enabled for a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SnapshotsEnabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-snapshot-configuration-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationSnapshotConfigurationDescription
---
