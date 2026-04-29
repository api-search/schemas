---
description: Provides details about a snapshot of application state.
layout: schema
name: SnapshotDetails
properties_list:
- description: ''
  name: SnapshotName
  type: object
- description: ''
  name: SnapshotStatus
  type: object
- description: ''
  name: ApplicationVersionId
  type: object
- description: ''
  name: SnapshotCreationTimestamp
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-snapshot-details-schema.json
slug: amazon-managed-apache-flink-snapshot-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-snapshot-details-schema.json\",\n  \"title\": \"SnapshotDetails\",\n  \"description\": \"Provides details about a snapshot of application state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotName\"\n        },\n        {\n          \"description\": \"The identifier for the application snapshot.\"\n        }\n      ]\n    },\n    \"SnapshotStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotStatus\"\n        },\n        {\n          \"description\": \"The status of the application snapshot.\"\n        }\n      ]\n    },\n    \"ApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\
  \n        },\n        {\n          \"description\": \"The current application version ID when the snapshot was created.\"\n        }\n      ]\n    },\n    \"SnapshotCreationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp of the application snapshot.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SnapshotName\",\n    \"SnapshotStatus\",\n    \"ApplicationVersionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-snapshot-details-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: SnapshotDetails
---
