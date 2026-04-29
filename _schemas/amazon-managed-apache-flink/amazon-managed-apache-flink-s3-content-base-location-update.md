---
description: The information required to update the S3 base location that holds the application.
layout: schema
name: S3ContentBaseLocationUpdate
properties_list:
- description: ''
  name: BucketARNUpdate
  type: object
- description: ''
  name: BasePathUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-s3-content-base-location-update-schema.json
slug: amazon-managed-apache-flink-s3-content-base-location-update
source_filename: amazon-managed-apache-flink-s3-content-base-location-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-content-base-location-update-schema.json\",\n  \"title\": \"S3ContentBaseLocationUpdate\",\n  \"description\": \"The information required to update the S3 base location that holds the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketARNUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketARN\"\n        },\n        {\n          \"description\": \"The updated Amazon Resource Name (ARN) of the S3 bucket.\"\n        }\n      ]\n    },\n    \"BasePathUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BasePath\"\n        },\n        {\n          \"description\": \"The updated S3 bucket path.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-content-base-location-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: S3ContentBaseLocationUpdate
---
