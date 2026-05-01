---
description: '<p>For a SQL-based Kinesis Data Analytics application, provides additional mapping information when the record format uses delimiters, such as CSV. For example, the following sample records use CSV format, where the records use the <i>''\n''</i> as the row delimiter and a comma (",") as the column delimiter: </p> <p> <code>"name1", "address1"</code> </p> <p> <code>"name2", "address2"</code> </p>'
layout: schema
name: CSVMappingParameters
properties_list:
- description: ''
  name: RecordRowDelimiter
  type: object
- description: ''
  name: RecordColumnDelimiter
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-csv-mapping-parameters-schema.json
slug: amazon-managed-apache-flink-csv-mapping-parameters
source_filename: amazon-managed-apache-flink-csv-mapping-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-csv-mapping-parameters-schema.json\",\n  \"title\": \"CSVMappingParameters\",\n  \"description\": \"<p>For a SQL-based Kinesis Data Analytics application, provides additional mapping information when the record format uses delimiters, such as CSV. For example, the following sample records use CSV format, where the records use the <i>'\\\\n'</i> as the row delimiter and a comma (\\\",\\\") as the column delimiter: </p> <p> <code>\\\"name1\\\", \\\"address1\\\"</code> </p> <p> <code>\\\"name2\\\", \\\"address2\\\"</code> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecordRowDelimiter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordRowDelimiter\"\n        },\n        {\n          \"description\": \"The row delimiter.\
  \ For example, in a CSV format, <i>'\\\\n'</i> is the typical row delimiter.\"\n        }\n      ]\n    },\n    \"RecordColumnDelimiter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordColumnDelimiter\"\n        },\n        {\n          \"description\": \"The column delimiter. For example, in a CSV format, a comma (\\\",\\\") is the typical column delimiter.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RecordRowDelimiter\",\n    \"RecordColumnDelimiter\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-csv-mapping-parameters-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CSVMappingParameters
---
