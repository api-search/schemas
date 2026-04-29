---
description: Information about S3 logs for a build project.
layout: schema
name: S3LogsConfig
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: encryptionDisabled
  type: object
- description: ''
  name: bucketOwnerAccess
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-s3-logs-config-schema.json
slug: amazon-codebuild-s3-logs-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-s3-logs-config-schema.json\",\n  \"title\": \"S3LogsConfig\",\n  \"description\": \" Information about S3 logs for a build project. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogsConfigStatusType\"\n        },\n        {\n          \"description\": \"<p>The current status of the S3 build logs. Valid values are:</p> <ul> <li> <p> <code>ENABLED</code>: S3 build logs are enabled for this build project.</p> </li> <li> <p> <code>DISABLED</code>: S3 build logs are not enabled for this build project.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\"\
  : \" The ARN of an S3 bucket and the path prefix for S3 logs. If your Amazon S3 bucket name is <code>my-bucket</code>, and your path prefix is <code>build-log</code>, then acceptable formats are <code>my-bucket/build-log</code> or <code>arn:aws:s3:::my-bucket/build-log</code>. \"\n        }\n      ]\n    },\n    \"encryptionDisabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \" Set to true if you do not want your S3 build log output encrypted. By default S3 build logs are encrypted. \"\n        }\n      ]\n    },\n    \"bucketOwnerAccess\": {\n      \"$ref\": \"#/components/schemas/BucketOwnerAccess\"\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-s3-logs-config-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: S3LogsConfig
---
