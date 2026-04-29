---
description: AddApplicationOutputResponse schema from Amazon Managed Service for Apache Flink API
layout: schema
name: AddApplicationOutputResponse
properties_list:
- description: ''
  name: ApplicationARN
  type: object
- description: ''
  name: ApplicationVersionId
  type: object
- description: ''
  name: OutputDescriptions
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-add-application-output-response-schema.json
slug: amazon-managed-apache-flink-add-application-output-response
source_filename: amazon-managed-apache-flink-add-application-output-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-output-response-schema.json\",\n  \"title\": \"AddApplicationOutputResponse\",\n  \"description\": \"AddApplicationOutputResponse schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The application Amazon Resource Name (ARN).\"\n        }\n      ]\n    },\n    \"ApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The updated application version ID. Kinesis Data Analytics increments this ID when the application\
  \ is updated.\"\n        }\n      ]\n    },\n    \"OutputDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputDescriptions\"\n        },\n        {\n          \"description\": \"Describes the application output configuration. For more information, see <a href=\\\"https://docs.aws.amazon.com/kinesisanalytics/latest/dev/how-it-works-output.html\\\">Configuring Application Output</a>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-output-response-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: AddApplicationOutputResponse
---
