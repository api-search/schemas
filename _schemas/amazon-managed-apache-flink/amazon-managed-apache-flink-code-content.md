---
description: Specifies either the application code, or the location of the application code, for a Flink-based Kinesis Data Analytics application.
layout: schema
name: CodeContent
properties_list:
- description: ''
  name: TextContent
  type: object
- description: ''
  name: ZipFileContent
  type: object
- description: ''
  name: S3ContentLocation
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-code-content-schema.json
slug: amazon-managed-apache-flink-code-content
source_filename: amazon-managed-apache-flink-code-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-code-content-schema.json\",\n  \"title\": \"CodeContent\",\n  \"description\": \"Specifies either the application code, or the location of the application code, for a Flink-based Kinesis Data Analytics application. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TextContent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TextContent\"\n        },\n        {\n          \"description\": \"The text-format code for a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"ZipFileContent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZipFileContent\"\n        },\n        {\n          \"description\": \"The zip-format code for a Flink-based Kinesis Data Analytics application.\"\
  \n        }\n      ]\n    },\n    \"S3ContentLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ContentLocation\"\n        },\n        {\n          \"description\": \"Information about the Amazon S3 bucket that contains the application code.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-code-content-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CodeContent
---
