---
description: Describes an update for the Amazon S3 code content location for an application.
layout: schema
name: S3ContentLocationUpdate
properties_list:
- description: ''
  name: BucketARNUpdate
  type: object
- description: ''
  name: FileKeyUpdate
  type: object
- description: ''
  name: ObjectVersionUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-s3-content-location-update-schema.json
slug: amazon-managed-apache-flink-s3-content-location-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-content-location-update-schema.json\",\n  \"title\": \"S3ContentLocationUpdate\",\n  \"description\": \"Describes an update for the Amazon S3 code content location for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketARNUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketARN\"\n        },\n        {\n          \"description\": \"The new Amazon Resource Name (ARN) for the S3 bucket containing the application code.\"\n        }\n      ]\n    },\n    \"FileKeyUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileKey\"\n        },\n        {\n          \"description\": \"The new file key for the object containing the application code.\"\n        }\n      ]\n\
  \    },\n    \"ObjectVersionUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectVersion\"\n        },\n        {\n          \"description\": \"The new version of the object containing the application code.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-content-location-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: S3ContentLocationUpdate
---
