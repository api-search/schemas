---
description: CreateApplicationPresignedUrlRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: CreateApplicationPresignedUrlRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: UrlType
  type: object
- description: ''
  name: SessionExpirationDurationInSeconds
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-create-application-presigned-url-request-schema.json
slug: amazon-managed-apache-flink-create-application-presigned-url-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-create-application-presigned-url-request-schema.json\",\n  \"title\": \"CreateApplicationPresignedUrlRequest\",\n  \"description\": \"CreateApplicationPresignedUrlRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application.\"\n        }\n      ]\n    },\n    \"UrlType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UrlType\"\n        },\n        {\n          \"description\": \"The type of the extension for which to create and return a URL. Currently, the only valid extension URL type\
  \ is <code>FLINK_DASHBOARD_URL</code>. \"\n        }\n      ]\n    },\n    \"SessionExpirationDurationInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionExpirationDurationInSeconds\"\n        },\n        {\n          \"description\": \"The duration in seconds for which the returned URL will be valid.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"UrlType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-create-application-presigned-url-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CreateApplicationPresignedUrlRequest
---
