---
description: When you update a reference data source configuration for a SQL-based Kinesis Data Analytics application, this object provides all the updated values (such as the source bucket name and object key name), the in-application table name that is created, and updated mapping information that maps the data in the Amazon S3 object to the in-application reference table that is created.
layout: schema
name: ReferenceDataSourceUpdate
properties_list:
- description: ''
  name: ReferenceId
  type: object
- description: ''
  name: TableNameUpdate
  type: object
- description: ''
  name: S3ReferenceDataSourceUpdate
  type: object
- description: ''
  name: ReferenceSchemaUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-reference-data-source-update-schema.json
slug: amazon-managed-apache-flink-reference-data-source-update
source_filename: amazon-managed-apache-flink-reference-data-source-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-reference-data-source-update-schema.json\",\n  \"title\": \"ReferenceDataSourceUpdate\",\n  \"description\": \"When you update a reference data source configuration for a SQL-based Kinesis Data Analytics application, this object provides all the updated values (such as the source bucket name and object key name), the in-application table name that is created, and updated mapping information that maps the data in the Amazon S3 object to the in-application reference table that is created.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReferenceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the reference data source that is being updated. You can use the\
  \ <a>DescribeApplication</a> operation to get this value.\"\n        }\n      ]\n    },\n    \"TableNameUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppTableName\"\n        },\n        {\n          \"description\": \"The in-application table name that is created by this update.\"\n        }\n      ]\n    },\n    \"S3ReferenceDataSourceUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ReferenceDataSourceUpdate\"\n        },\n        {\n          \"description\": \"Describes the S3 bucket name, object key name, and IAM role that Kinesis Data Analytics can assume to read the Amazon S3 object on your behalf and populate the in-application reference table.\"\n        }\n      ]\n    },\n    \"ReferenceSchemaUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceSchema\"\n        },\n        {\n          \"description\": \"Describes the format of the data in the streaming\
  \ source, and how each data element maps to corresponding columns created in the in-application stream. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ReferenceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-reference-data-source-update-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ReferenceDataSourceUpdate
---
