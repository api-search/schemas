---
description: ListApplicationSnapshotsResponse schema from Amazon Managed Service for Apache Flink API
layout: schema
name: ListApplicationSnapshotsResponse
properties_list:
- description: ''
  name: SnapshotSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-list-application-snapshots-response-schema.json
slug: amazon-managed-apache-flink-list-application-snapshots-response
source_filename: amazon-managed-apache-flink-list-application-snapshots-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-list-application-snapshots-response-schema.json\",\n  \"title\": \"ListApplicationSnapshotsResponse\",\n  \"description\": \"ListApplicationSnapshotsResponse schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotSummaries\"\n        },\n        {\n          \"description\": \"A collection of objects containing information about the application snapshots.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or <code>null</code>\
  \ if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-list-application-snapshots-response-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ListApplicationSnapshotsResponse
---
