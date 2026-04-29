---
description: For a SQL-based Kinesis Data Analytics application, describes the reference data source by providing the source information (Amazon S3 bucket name and object key name), the resulting in-application table name that is created, and the necessary schema to map the data elements in the Amazon S3 object to the in-application table.
layout: schema
name: ReferenceDataSource
properties_list:
- description: ''
  name: TableName
  type: object
- description: ''
  name: S3ReferenceDataSource
  type: object
- description: ''
  name: ReferenceSchema
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-reference-data-source-schema.json
slug: amazon-managed-apache-flink-reference-data-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-reference-data-source-schema.json\",\n  \"title\": \"ReferenceDataSource\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, describes the reference data source by providing the source information (Amazon S3 bucket name and object key name), the resulting in-application table name that is created, and the necessary schema to map the data elements in the Amazon S3 object to the in-application table.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppTableName\"\n        },\n        {\n          \"description\": \"The name of the in-application table to create.\"\n        }\n      ]\n    },\n    \"S3ReferenceDataSource\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/S3ReferenceDataSource\"\n        },\n        {\n          \"description\": \"Identifies the S3 bucket and object that contains the reference data. A Kinesis Data Analytics application loads reference data only once. If the data changes, you call the <a>UpdateApplication</a> operation to trigger reloading of data into your application. \"\n        }\n      ]\n    },\n    \"ReferenceSchema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceSchema\"\n        },\n        {\n          \"description\": \"Describes the format of the data in the streaming source, and how each data element maps to corresponding columns created in the in-application stream.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TableName\",\n    \"ReferenceSchema\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-reference-data-source-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ReferenceDataSource
---
