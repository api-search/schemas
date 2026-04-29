---
description: CreateTrailRequest schema
layout: schema
name: CreateTrailRequest
properties_list:
- description: The name of the trail.
  name: Name
  type: string
- description: The name of the S3 bucket for log file delivery.
  name: S3BucketName
  type: string
- description: The S3 key prefix for log file delivery.
  name: S3KeyPrefix
  type: string
- description: Whether the trail is created in all regions.
  name: IsMultiRegionTrail
  type: boolean
- description: Whether log file integrity validation is enabled.
  name: EnableLogFileValidation
  type: boolean
- description: The ARN of the CloudWatch Logs log group.
  name: CloudWatchLogsLogGroupArn
  type: string
- description: The role ARN for CloudWatch Logs delivery.
  name: CloudWatchLogsRoleArn
  type: string
provider_name: Amazon CloudTrail
provider_slug: amazon-cloudtrail
schema_file: json-schema/cloudtrail-create-trail-request-schema.json
slug: cloudtrail-create-trail-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-create-trail-request-schema.json\",\n  \"title\": \"CreateTrailRequest\",\n  \"description\": \"CreateTrailRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the trail.\"\n    },\n    \"S3BucketName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the S3 bucket for log file delivery.\"\n    },\n    \"S3KeyPrefix\": {\n      \"type\": \"string\",\n      \"description\": \"The S3 key prefix for log file delivery.\"\n    },\n    \"IsMultiRegionTrail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the trail is created in all regions.\"\n    },\n    \"EnableLogFileValidation\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether log file integrity\
  \ validation is enabled.\"\n    },\n    \"CloudWatchLogsLogGroupArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the CloudWatch Logs log group.\"\n    },\n    \"CloudWatchLogsRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The role ARN for CloudWatch Logs delivery.\"\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"S3BucketName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-create-trail-request-schema.json
tags:
- AWS
- CloudTrail
- Audit
- Compliance
- Governance
- Security
title: CreateTrailRequest
---
