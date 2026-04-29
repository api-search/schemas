---
description: DescribeApplicationSnapshotResponse schema from Amazon Managed Service for Apache Flink API
layout: schema
name: DescribeApplicationSnapshotResponse
properties_list:
- description: ''
  name: SnapshotDetails
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-describe-application-snapshot-response-schema.json
slug: amazon-managed-apache-flink-describe-application-snapshot-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-describe-application-snapshot-response-schema.json\",\n  \"title\": \"DescribeApplicationSnapshotResponse\",\n  \"description\": \"DescribeApplicationSnapshotResponse schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotDetails\"\n        },\n        {\n          \"description\": \"An object containing information about the application snapshot.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SnapshotDetails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-describe-application-snapshot-response-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DescribeApplicationSnapshotResponse
---
