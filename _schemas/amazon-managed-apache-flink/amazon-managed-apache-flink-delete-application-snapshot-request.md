---
description: DeleteApplicationSnapshotRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: DeleteApplicationSnapshotRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: SnapshotName
  type: object
- description: ''
  name: SnapshotCreationTimestamp
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-delete-application-snapshot-request-schema.json
slug: amazon-managed-apache-flink-delete-application-snapshot-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-snapshot-request-schema.json\",\n  \"title\": \"DeleteApplicationSnapshotRequest\",\n  \"description\": \"DeleteApplicationSnapshotRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of an existing application.\"\n        }\n      ]\n    },\n    \"SnapshotName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotName\"\n        },\n        {\n          \"description\": \"The identifier for the snapshot delete.\"\n        }\n      ]\n    },\n    \"SnapshotCreationTimestamp\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The creation timestamp of the application snapshot to delete. You can retrieve this value using or .\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"SnapshotName\",\n    \"SnapshotCreationTimestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-snapshot-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DeleteApplicationSnapshotRequest
---
