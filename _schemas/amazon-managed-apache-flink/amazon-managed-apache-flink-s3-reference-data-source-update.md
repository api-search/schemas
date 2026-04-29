---
description: For a SQL-based Kinesis Data Analytics application, describes the Amazon S3 bucket name and object key name for an in-application reference table.
layout: schema
name: S3ReferenceDataSourceUpdate
properties_list:
- description: ''
  name: BucketARNUpdate
  type: object
- description: ''
  name: FileKeyUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-s3-reference-data-source-update-schema.json
slug: amazon-managed-apache-flink-s3-reference-data-source-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-reference-data-source-update-schema.json\",\n  \"title\": \"S3ReferenceDataSourceUpdate\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, describes the Amazon S3 bucket name and object key name for an in-application reference table. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketARNUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the S3 bucket.\"\n        }\n      ]\n    },\n    \"FileKeyUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileKey\"\n        },\n        {\n          \"description\": \"The object key name.\"\n        }\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-reference-data-source-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: S3ReferenceDataSourceUpdate
---
