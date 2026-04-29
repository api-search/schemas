---
description: <p>For a SQL-based Kinesis Data Analytics application, describes the mapping of each data element in the streaming source to the corresponding column in the in-application stream.</p> <p>Also used to describe the format of the reference data source.</p>
layout: schema
name: RecordColumn
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Mapping
  type: object
- description: ''
  name: SqlType
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-record-column-schema.json
slug: amazon-managed-apache-flink-record-column
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-record-column-schema.json\",\n  \"title\": \"RecordColumn\",\n  \"description\": \"<p>For a SQL-based Kinesis Data Analytics application, describes the mapping of each data element in the streaming source to the corresponding column in the in-application stream.</p> <p>Also used to describe the format of the reference data source.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordColumnName\"\n        },\n        {\n          \"description\": \"The name of the column that is created in the in-application input stream or reference table.\"\n        }\n      ]\n    },\n    \"Mapping\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordColumnMapping\"\
  \n        },\n        {\n          \"description\": \"A reference to the data element in the streaming input or the reference data source.\"\n        }\n      ]\n    },\n    \"SqlType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordColumnSqlType\"\n        },\n        {\n          \"description\": \"The type of column created in the in-application input stream or reference table.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"SqlType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-record-column-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: RecordColumn
---
