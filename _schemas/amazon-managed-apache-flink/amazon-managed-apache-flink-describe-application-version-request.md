---
description: DescribeApplicationVersionRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: DescribeApplicationVersionRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: ApplicationVersionId
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-describe-application-version-request-schema.json
slug: amazon-managed-apache-flink-describe-application-version-request
source_filename: amazon-managed-apache-flink-describe-application-version-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-describe-application-version-request-schema.json\",\n  \"title\": \"DescribeApplicationVersionRequest\",\n  \"description\": \"DescribeApplicationVersionRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application for which you want to get the version description.\"\n        }\n      ]\n    },\n    \"ApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The ID of the application version for which\
  \ you want to get the description.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"ApplicationVersionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-describe-application-version-request-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DescribeApplicationVersionRequest
---
