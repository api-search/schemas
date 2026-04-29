---
description: Describes details about the code of a Kinesis Data Analytics application.
layout: schema
name: CodeContentDescription
properties_list:
- description: ''
  name: TextContent
  type: object
- description: ''
  name: CodeMD5
  type: object
- description: ''
  name: CodeSize
  type: object
- description: ''
  name: S3ApplicationCodeLocationDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-code-content-description-schema.json
slug: amazon-managed-apache-flink-code-content-description
source_filename: amazon-managed-apache-flink-code-content-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-code-content-description-schema.json\",\n  \"title\": \"CodeContentDescription\",\n  \"description\": \"Describes details about the code of a Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TextContent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TextContent\"\n        },\n        {\n          \"description\": \"The text-format code\"\n        }\n      ]\n    },\n    \"CodeMD5\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeMD5\"\n        },\n        {\n          \"description\": \"The checksum that can be used to validate zip-format code.\"\n        }\n      ]\n    },\n    \"CodeSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeSize\"\
  \n        },\n        {\n          \"description\": \"The size in bytes of the application code. Can be used to validate zip-format code.\"\n        }\n      ]\n    },\n    \"S3ApplicationCodeLocationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ApplicationCodeLocationDescription\"\n        },\n        {\n          \"description\": \"The S3 bucket Amazon Resource Name (ARN), file key, and object version of the application code stored in Amazon S3.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-code-content-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CodeContentDescription
---
