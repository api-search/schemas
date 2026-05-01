---
description: AddApplicationInputRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: AddApplicationInputRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: CurrentApplicationVersionId
  type: object
- description: ''
  name: Input
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-add-application-input-request-schema.json
slug: amazon-managed-apache-flink-add-application-input-request
source_filename: amazon-managed-apache-flink-add-application-input-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-input-request-schema.json\",\n  \"title\": \"AddApplicationInputRequest\",\n  \"description\": \"AddApplicationInputRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of your existing application to which you want to add the streaming source.\"\n        }\n      ]\n    },\n    \"CurrentApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The current version of your application. You must\
  \ provide the <code>ApplicationVersionID</code> or the <code>ConditionalToken</code>.You can use the <a>DescribeApplication</a> operation to find the current application version.\"\n        }\n      ]\n    },\n    \"Input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Input\"\n        },\n        {\n          \"description\": \"The <a>Input</a> to add.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"CurrentApplicationVersionId\",\n    \"Input\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-input-request-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: AddApplicationInputRequest
---
