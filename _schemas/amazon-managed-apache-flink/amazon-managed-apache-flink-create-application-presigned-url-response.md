---
description: CreateApplicationPresignedUrlResponse schema from Amazon Managed Service for Apache Flink API
layout: schema
name: CreateApplicationPresignedUrlResponse
properties_list:
- description: ''
  name: AuthorizedUrl
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-create-application-presigned-url-response-schema.json
slug: amazon-managed-apache-flink-create-application-presigned-url-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-create-application-presigned-url-response-schema.json\",\n  \"title\": \"CreateApplicationPresignedUrlResponse\",\n  \"description\": \"CreateApplicationPresignedUrlResponse schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuthorizedUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizedUrl\"\n        },\n        {\n          \"description\": \"The URL of the extension.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-create-application-presigned-url-response-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CreateApplicationPresignedUrlResponse
---
