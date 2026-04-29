---
description: Actions to execute after the instance launches
layout: schema
name: PostLaunchActions
properties_list:
- description: Deployment type for post-launch actions
  name: deployment
  type: string
- description: S3 bucket for action logs
  name: s3LogBucket
  type: string
- description: S3 key prefix for action logs
  name: s3OutputKeyPrefix
  type: string
- description: CloudWatch log group name
  name: cloudWatchLogGroupName
  type: string
- description: SSM documents to execute
  name: ssmDocuments
  type: array
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-post-launch-actions-schema.json
slug: application-migration-service-post-launch-actions
source_filename: application-migration-service-post-launch-actions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-post-launch-actions-schema.json\",\n  \"title\": \"PostLaunchActions\",\n  \"description\": \"Actions to execute after the instance launches\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deployment\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment type for post-launch actions\"\n    },\n    \"s3LogBucket\": {\n      \"type\": \"string\",\n      \"description\": \"S3 bucket for action logs\"\n    },\n    \"s3OutputKeyPrefix\": {\n      \"type\": \"string\",\n      \"description\": \"S3 key prefix for action logs\"\n    },\n    \"cloudWatchLogGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"CloudWatch log group name\"\n    },\n    \"ssmDocuments\": {\n      \"type\": \"array\",\n      \"description\": \"SSM documents to execute\"\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-post-launch-actions-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: PostLaunchActions
---
