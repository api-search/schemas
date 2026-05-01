---
description: <p>For a SQL-based Kinesis Data Analytics application, identifies the Amazon S3 bucket and object that contains the reference data.</p> <p>A Kinesis Data Analytics application loads reference data only once. If the data changes, you call the <a>UpdateApplication</a> operation to trigger reloading of data into your application. </p>
layout: schema
name: S3ReferenceDataSource
properties_list:
- description: ''
  name: BucketARN
  type: object
- description: ''
  name: FileKey
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-s3-reference-data-source-schema.json
slug: amazon-managed-apache-flink-s3-reference-data-source
source_filename: amazon-managed-apache-flink-s3-reference-data-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-reference-data-source-schema.json\",\n  \"title\": \"S3ReferenceDataSource\",\n  \"description\": \"<p>For a SQL-based Kinesis Data Analytics application, identifies the Amazon S3 bucket and object that contains the reference data.</p> <p>A Kinesis Data Analytics application loads reference data only once. If the data changes, you call the <a>UpdateApplication</a> operation to trigger reloading of data into your application. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the S3 bucket.\"\n        }\n      ]\n    },\n    \"FileKey\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/FileKey\"\n        },\n        {\n          \"description\": \"The object key name containing the reference data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-reference-data-source-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: S3ReferenceDataSource
---
