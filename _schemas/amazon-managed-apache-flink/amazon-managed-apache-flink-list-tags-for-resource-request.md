---
description: ListTagsForResourceRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: ListTagsForResourceRequest
properties_list:
- description: ''
  name: ResourceARN
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-list-tags-for-resource-request-schema.json
slug: amazon-managed-apache-flink-list-tags-for-resource-request
source_filename: amazon-managed-apache-flink-list-tags-for-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-list-tags-for-resource-request-schema.json\",\n  \"title\": \"ListTagsForResourceRequest\",\n  \"description\": \"ListTagsForResourceRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisAnalyticsARN\"\n        },\n        {\n          \"description\": \"The ARN of the application for which to retrieve tags.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-list-tags-for-resource-request-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ListTagsForResourceRequest
---
