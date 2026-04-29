---
description: RollbackApplicationRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: RollbackApplicationRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: CurrentApplicationVersionId
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-rollback-application-request-schema.json
slug: amazon-managed-apache-flink-rollback-application-request
source_filename: amazon-managed-apache-flink-rollback-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-rollback-application-request-schema.json\",\n  \"title\": \"RollbackApplicationRequest\",\n  \"description\": \"RollbackApplicationRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application.\"\n        }\n      ]\n    },\n    \"CurrentApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The current application version ID. You can retrieve the application version ID using <a>DescribeApplication</a>.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"CurrentApplicationVersionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-rollback-application-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: RollbackApplicationRequest
---
