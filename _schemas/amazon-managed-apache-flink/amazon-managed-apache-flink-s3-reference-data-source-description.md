---
description: For a SQL-based Kinesis Data Analytics application, provides the bucket name and object key name that stores the reference data.
layout: schema
name: S3ReferenceDataSourceDescription
properties_list:
- description: ''
  name: BucketARN
  type: object
- description: ''
  name: FileKey
  type: object
- description: ''
  name: ReferenceRoleARN
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-s3-reference-data-source-description-schema.json
slug: amazon-managed-apache-flink-s3-reference-data-source-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-reference-data-source-description-schema.json\",\n  \"title\": \"S3ReferenceDataSourceDescription\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, provides the bucket name and object key name that stores the reference data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the S3 bucket.\"\n        }\n      ]\n    },\n    \"FileKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileKey\"\n        },\n        {\n          \"description\": \"Amazon S3 object key name.\"\n        }\n      ]\n    },\n    \"ReferenceRoleARN\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"<p>The ARN of the IAM role that Kinesis Data Analytics can assume to read the Amazon S3 object on your behalf to populate the in-application reference table. </p> <note> <p>Provided for backward compatibility. Applications that are created with the current API version have an application-level service execution role rather than a resource-level role.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BucketARN\",\n    \"FileKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-s3-reference-data-source-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: S3ReferenceDataSourceDescription
---
