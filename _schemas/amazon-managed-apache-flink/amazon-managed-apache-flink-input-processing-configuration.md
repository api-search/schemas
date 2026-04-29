---
description: For a SQL-based Kinesis Data Analytics application, describes a processor that is used to preprocess the records in the stream before being processed by your application code. Currently, the only input processor available is <a href="https://docs.aws.amazon.com/lambda/">Amazon Lambda</a>.
layout: schema
name: InputProcessingConfiguration
properties_list:
- description: ''
  name: InputLambdaProcessor
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-input-processing-configuration-schema.json
slug: amazon-managed-apache-flink-input-processing-configuration
source_filename: amazon-managed-apache-flink-input-processing-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-processing-configuration-schema.json\",\n  \"title\": \"InputProcessingConfiguration\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, describes a processor that is used to preprocess the records in the stream before being processed by your application code. Currently, the only input processor available is <a href=\\\"https://docs.aws.amazon.com/lambda/\\\">Amazon Lambda</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputLambdaProcessor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLambdaProcessor\"\n        },\n        {\n          \"description\": \"The <a>InputLambdaProcessor</a> that is used to preprocess the records in the stream before being processed by your application\
  \ code.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InputLambdaProcessor\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-processing-configuration-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: InputProcessingConfiguration
---
