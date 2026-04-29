---
description: The description of the S3 base location that holds the application.
layout: schema
name: S3ContentBaseLocationDescription
properties_list:
- description: ''
  name: BucketARN
  type: object
- description: ''
  name: BasePath
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-s3-content-base-location-description-schema.json
slug: amazon-managed-apache-flink-s3-content-base-location-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-content-base-location-description-schema.json\",\n  \"title\": \"S3ContentBaseLocationDescription\",\n  \"description\": \"The description of the S3 base location that holds the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the S3 bucket.\"\n        }\n      ]\n    },\n    \"BasePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BasePath\"\n        },\n        {\n          \"description\": \"The base path for the S3 bucket.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BucketARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-content-base-location-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: S3ContentBaseLocationDescription
---
