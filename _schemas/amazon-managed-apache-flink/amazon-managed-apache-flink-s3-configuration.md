---
description: For a SQL-based Kinesis Data Analytics application, provides a description of an Amazon S3 data source, including the Amazon Resource Name (ARN) of the S3 bucket and the name of the Amazon S3 object that contains the data.
layout: schema
name: S3Configuration
properties_list:
- description: ''
  name: BucketARN
  type: object
- description: ''
  name: FileKey
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-s3-configuration-schema.json
slug: amazon-managed-apache-flink-s3-configuration
source_filename: amazon-managed-apache-flink-s3-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-configuration-schema.json\",\n  \"title\": \"S3Configuration\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, provides a description of an Amazon S3 data source, including the Amazon Resource Name (ARN) of the S3 bucket and the name of the Amazon S3 object that contains the data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketARN\"\n        },\n        {\n          \"description\": \"The ARN of the S3 bucket that contains the data.\"\n        }\n      ]\n    },\n    \"FileKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileKey\"\n        },\n        {\n          \"description\": \"The name of the\
  \ object that contains the data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BucketARN\",\n    \"FileKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-configuration-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: S3Configuration
---
