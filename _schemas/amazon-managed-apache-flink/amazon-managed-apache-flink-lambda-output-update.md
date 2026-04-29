---
description: When you update an SQL-based Kinesis Data Analytics application's output configuration using the <a>UpdateApplication</a> operation, provides information about an Amazon Lambda function that is configured as the destination.
layout: schema
name: LambdaOutputUpdate
properties_list:
- description: ''
  name: ResourceARNUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-lambda-output-update-schema.json
slug: amazon-managed-apache-flink-lambda-output-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-lambda-output-update-schema.json\",\n  \"title\": \"LambdaOutputUpdate\",\n  \"description\": \"When you update an SQL-based Kinesis Data Analytics application's output configuration using the <a>UpdateApplication</a> operation, provides information about an Amazon Lambda function that is configured as the destination.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARNUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the destination Amazon Lambda function.</p> <note> <p>To specify an earlier version of the Lambda function than the latest, include the Lambda function version in the Lambda function ARN. For more\
  \ information about Lambda ARNs, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html#arn-syntax-lambda\\\">Example ARNs: Amazon Lambda</a> </p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceARNUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-lambda-output-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: LambdaOutputUpdate
---
