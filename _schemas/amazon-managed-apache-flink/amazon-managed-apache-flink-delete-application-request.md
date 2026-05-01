---
description: DeleteApplicationRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: DeleteApplicationRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: CreateTimestamp
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-delete-application-request-schema.json
slug: amazon-managed-apache-flink-delete-application-request
source_filename: amazon-managed-apache-flink-delete-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-request-schema.json\",\n  \"title\": \"DeleteApplicationRequest\",\n  \"description\": \"DeleteApplicationRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application to delete.\"\n        }\n      ]\n    },\n    \"CreateTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Use the <code>DescribeApplication</code> operation to get this value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"ApplicationName\",\n    \"CreateTimestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-request-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DeleteApplicationRequest
---
