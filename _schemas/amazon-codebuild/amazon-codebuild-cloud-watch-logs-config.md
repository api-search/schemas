---
description: Information about CloudWatch Logs for a build project.
layout: schema
name: CloudWatchLogsConfig
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: groupName
  type: object
- description: ''
  name: streamName
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-cloud-watch-logs-config-schema.json
slug: amazon-codebuild-cloud-watch-logs-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-cloud-watch-logs-config-schema.json\",\n  \"title\": \"CloudWatchLogsConfig\",\n  \"description\": \" Information about CloudWatch Logs for a build project. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogsConfigStatusType\"\n        },\n        {\n          \"description\": \"<p>The current status of the logs in CloudWatch Logs for a build project. Valid values are:</p> <ul> <li> <p> <code>ENABLED</code>: CloudWatch Logs are enabled for this build project.</p> </li> <li> <p> <code>DISABLED</code>: CloudWatch Logs are not enabled for this build project.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"groupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \" The group name of the logs in CloudWatch Logs. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/Working-with-log-groups-and-streams.html\\\">Working with Log Groups and Log Streams</a>. \"\n        }\n      ]\n    },\n    \"streamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The prefix of the stream name of the CloudWatch Logs. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/Working-with-log-groups-and-streams.html\\\">Working with Log Groups and Log Streams</a>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-cloud-watch-logs-config-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: CloudWatchLogsConfig
---
