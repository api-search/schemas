---
description: Container for specifying the Lambda notification configuration.
layout: schema
name: CloudFunctionConfiguration
properties_list:
- description: An optional unique identifier for configurations in a notification configuration. If you don't provide one, Amazon S3 will assign an ID.
  name: Id
  type: string
- description: ''
  name: Event
  type: object
- description: ''
  name: Events
  type: object
- description: ''
  name: CloudFunction
  type: object
- description: ''
  name: InvocationRole
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-cloudfunctionconfiguration-schema.json
slug: s3-cloudfunctionconfiguration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CloudFunctionConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"An optional unique identifier for configurations in a notification configuration. If you don't provide one, Amazon S3 will assign an ID.\"\n    },\n    \"Event\": {},\n    \"Events\": {},\n    \"CloudFunction\": {},\n    \"InvocationRole\": {}\n  },\n  \"description\": \"Container for specifying the Lambda notification configuration.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-cloudfunctionconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: CloudFunctionConfiguration
---
