---
description: For a SQL-based Kinesis Data Analytics application, provides the configuration information about an input processor. Currently, the only input processor available is <a href="https://docs.aws.amazon.com/lambda/">Amazon Lambda</a>.
layout: schema
name: InputProcessingConfigurationDescription
properties_list:
- description: ''
  name: InputLambdaProcessorDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-input-processing-configuration-description-schema.json
slug: amazon-managed-apache-flink-input-processing-configuration-description
source_filename: amazon-managed-apache-flink-input-processing-configuration-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-processing-configuration-description-schema.json\",\n  \"title\": \"InputProcessingConfigurationDescription\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, provides the configuration information about an input processor. Currently, the only input processor available is <a href=\\\"https://docs.aws.amazon.com/lambda/\\\">Amazon Lambda</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputLambdaProcessorDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLambdaProcessorDescription\"\n        },\n        {\n          \"description\": \"Provides configuration information about the associated <a>InputLambdaProcessorDescription</a> \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-processing-configuration-description-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: InputProcessingConfigurationDescription
---
