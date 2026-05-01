---
description: For a SQL-based Kinesis Data Analytics application, an object that contains the Amazon Resource Name (ARN) of the Amazon Lambda function that is used to preprocess records in the stream.
layout: schema
name: InputLambdaProcessorDescription
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: RoleARN
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-input-lambda-processor-description-schema.json
slug: amazon-managed-apache-flink-input-lambda-processor-description
source_filename: amazon-managed-apache-flink-input-lambda-processor-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-lambda-processor-description-schema.json\",\n  \"title\": \"InputLambdaProcessorDescription\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, an object that contains the Amazon Resource Name (ARN) of the Amazon Lambda function that is used to preprocess records in the stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"<p>The ARN of the Amazon Lambda function that is used to preprocess the records in the stream.</p> <note> <p>To specify an earlier version of the Lambda function than the latest, include the Lambda function version in the Lambda function ARN. For more\
  \ information about Lambda ARNs, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html#arn-syntax-lambda\\\">Example ARNs: Amazon Lambda</a> </p> </note>\"\n        }\n      ]\n    },\n    \"RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"<p>The ARN of the IAM role that is used to access the Amazon Lambda function.</p> <note> <p>Provided for backward compatibility. Applications that are created with the current API version have an application-level service execution role rather than a resource-level role.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-lambda-processor-description-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: InputLambdaProcessorDescription
---
