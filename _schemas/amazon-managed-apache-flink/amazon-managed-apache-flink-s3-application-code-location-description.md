---
description: Describes the location of an application's code stored in an S3 bucket.
layout: schema
name: S3ApplicationCodeLocationDescription
properties_list:
- description: ''
  name: BucketARN
  type: object
- description: ''
  name: FileKey
  type: object
- description: ''
  name: ObjectVersion
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-s3-application-code-location-description-schema.json
slug: amazon-managed-apache-flink-s3-application-code-location-description
source_filename: amazon-managed-apache-flink-s3-application-code-location-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-application-code-location-description-schema.json\",\n  \"title\": \"S3ApplicationCodeLocationDescription\",\n  \"description\": \"Describes the location of an application's code stored in an S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the S3 bucket containing the application code.\"\n        }\n      ]\n    },\n    \"FileKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileKey\"\n        },\n        {\n          \"description\": \"The file key for the object containing the application code.\"\n        }\n      ]\n \
  \   },\n    \"ObjectVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectVersion\"\n        },\n        {\n          \"description\": \"The version of the object containing the application code.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BucketARN\",\n    \"FileKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-application-code-location-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: S3ApplicationCodeLocationDescription
---
