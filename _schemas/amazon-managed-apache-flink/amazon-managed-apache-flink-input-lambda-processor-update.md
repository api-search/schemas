---
description: For a SQL-based Kinesis Data Analytics application, represents an update to the <a>InputLambdaProcessor</a> that is used to preprocess the records in the stream.
layout: schema
name: InputLambdaProcessorUpdate
properties_list:
- description: ''
  name: ResourceARNUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-input-lambda-processor-update-schema.json
slug: amazon-managed-apache-flink-input-lambda-processor-update
source_filename: amazon-managed-apache-flink-input-lambda-processor-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-lambda-processor-update-schema.json\",\n  \"title\": \"InputLambdaProcessorUpdate\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, represents an update to the <a>InputLambdaProcessor</a> that is used to preprocess the records in the stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARNUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the new Amazon Lambda function that is used to preprocess the records in the stream.</p> <note> <p>To specify an earlier version of the Lambda function than the latest, include the Lambda function version in the Lambda function ARN. For more\
  \ information about Lambda ARNs, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html#arn-syntax-lambda\\\">Example ARNs: Amazon Lambda</a> </p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceARNUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-lambda-processor-update-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: InputLambdaProcessorUpdate
---
