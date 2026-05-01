---
description: TagResourceRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-tag-resource-request-schema.json
slug: amazon-managed-apache-flink-tag-resource-request
source_filename: amazon-managed-apache-flink-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisAnalyticsARN\"\n        },\n        {\n          \"description\": \"The ARN of the application to assign the tags.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"The key-value tags to assign to the application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceARN\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-tag-resource-request-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: TagResourceRequest
---
