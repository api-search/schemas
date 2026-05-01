---
description: Logging configuration for a GraphQL API
layout: schema
name: LogConfig
properties_list:
- description: CloudWatch Logs role ARN
  name: cloudWatchLogsRoleArn
  type: string
- description: Field log level
  name: fieldLogLevel
  type: string
- description: Whether to exclude verbose content
  name: excludeVerboseContent
  type: boolean
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-log-config-schema.json
slug: appsync-log-config
source_filename: appsync-log-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-log-config-schema.json\",\n  \"title\": \"LogConfig\",\n  \"description\": \"Logging configuration for a GraphQL API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cloudWatchLogsRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"CloudWatch Logs role ARN\"\n    },\n    \"fieldLogLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Field log level\"\n    },\n    \"excludeVerboseContent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to exclude verbose content\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-log-config-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: LogConfig
---
