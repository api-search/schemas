---
description: The logging parameters of a user pool.
layout: schema
name: LogConfigurationType
properties_list:
- description: ''
  name: LogLevel
  type: object
- description: ''
  name: EventSource
  type: object
- description: ''
  name: CloudWatchLogsConfiguration
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-log-configuration-type-schema.json
slug: user-pools-log-configuration-type
source_filename: user-pools-log-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-log-configuration-type-schema.json\",\n  \"title\": \"LogConfigurationType\",\n  \"description\": \"The logging parameters of a user pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"description\": \"The <code>errorlevel</code> selection of logs that a user pool sends for detailed activity logging.\"\n        }\n      ]\n    },\n    \"EventSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventSourceName\"\n        },\n        {\n          \"description\": \"The source of events that your user pool sends for detailed activity logging.\"\n        }\n      ]\n    },\n    \"CloudWatchLogsConfiguration\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLogsConfigurationType\"\n        },\n        {\n          \"description\": \"The CloudWatch logging destination of a user pool.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LogLevel\",\n    \"EventSource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-log-configuration-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: LogConfigurationType
---
