---
description: The CloudWatch logging destination of a user pool detailed activity logging configuration.
layout: schema
name: CloudWatchLogsConfigurationType
properties_list:
- description: ''
  name: LogGroupArn
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-cloud-watch-logs-configuration-type-schema.json
slug: user-pools-cloud-watch-logs-configuration-type
source_filename: user-pools-cloud-watch-logs-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-cloud-watch-logs-configuration-type-schema.json\",\n  \"title\": \"CloudWatchLogsConfigurationType\",\n  \"description\": \"The CloudWatch logging destination of a user pool detailed activity logging configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of a CloudWatch Logs log group where your user pool sends logs. The log group must not be encrypted with Key Management Service and must be in the same Amazon Web Services account as your user pool.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-cloud-watch-logs-configuration-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: CloudWatchLogsConfigurationType
---
