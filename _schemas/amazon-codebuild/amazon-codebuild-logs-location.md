---
description: Information about build logs in CloudWatch Logs.
layout: schema
name: LogsLocation
properties_list:
- description: ''
  name: groupName
  type: object
- description: ''
  name: streamName
  type: object
- description: ''
  name: deepLink
  type: object
- description: ''
  name: s3DeepLink
  type: object
- description: ''
  name: cloudWatchLogsArn
  type: object
- description: ''
  name: s3LogsArn
  type: object
- description: ''
  name: cloudWatchLogs
  type: object
- description: ''
  name: s3Logs
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-logs-location-schema.json
slug: amazon-codebuild-logs-location
source_filename: amazon-codebuild-logs-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-logs-location-schema.json\",\n  \"title\": \"LogsLocation\",\n  \"description\": \"Information about build logs in CloudWatch Logs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the CloudWatch Logs group for the build logs.\"\n        }\n      ]\n    },\n    \"streamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the CloudWatch Logs stream for the build logs.\"\n        }\n      ]\n    },\n    \"deepLink\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n\
  \        {\n          \"description\": \"The URL to an individual build log in CloudWatch Logs.\"\n        }\n      ]\n    },\n    \"s3DeepLink\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The URL to a build log in an S3 bucket. \"\n        }\n      ]\n    },\n    \"cloudWatchLogsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The ARN of CloudWatch Logs for a build project. Its format is <code>arn:${Partition}:logs:${Region}:${Account}:log-group:${LogGroupName}:log-stream:${LogStreamName}</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/list_amazoncloudwatchlogs.html#amazoncloudwatchlogs-resources-for-iam-policies\\\">Resources Defined by CloudWatch Logs</a>. \"\n        }\n      ]\n    },\n    \"s3LogsArn\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The ARN of S3 logs for a build project. Its format is <code>arn:${Partition}:s3:::${BucketName}/${ObjectName}</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/list_amazons3.html#amazons3-resources-for-iam-policies\\\">Resources Defined by Amazon S3</a>. \"\n        }\n      ]\n    },\n    \"cloudWatchLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLogsConfig\"\n        },\n        {\n          \"description\": \" Information about CloudWatch Logs for a build project. \"\n        }\n      ]\n    },\n    \"s3Logs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3LogsConfig\"\n        },\n        {\n          \"description\": \" Information about S3 logs for a build project. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-logs-location-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: LogsLocation
---
