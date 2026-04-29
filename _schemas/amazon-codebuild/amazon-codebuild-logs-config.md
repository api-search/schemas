---
description: Information about logs for a build project. These can be logs in CloudWatch Logs, built in a specified S3 bucket, or both.
layout: schema
name: LogsConfig
properties_list:
- description: ''
  name: cloudWatchLogs
  type: object
- description: ''
  name: s3Logs
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-logs-config-schema.json
slug: amazon-codebuild-logs-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-logs-config-schema.json\",\n  \"title\": \"LogsConfig\",\n  \"description\": \" Information about logs for a build project. These can be logs in CloudWatch Logs, built in a specified S3 bucket, or both. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cloudWatchLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLogsConfig\"\n        },\n        {\n          \"description\": \" Information about CloudWatch Logs for a build project. CloudWatch Logs are enabled by default. \"\n        }\n      ]\n    },\n    \"s3Logs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3LogsConfig\"\n        },\n        {\n          \"description\": \" Information about logs built to an S3 bucket for a build project. S3 logs\
  \ are not enabled by default. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-logs-config-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: LogsConfig
---
