---
description: ''
layout: schema
name: JobDescriptor
properties_list:
- description: ''
  name: JobId
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: Operation
  type: object
- description: ''
  name: Manifest
  type: object
- description: ''
  name: Priority
  type: integer
- description: ''
  name: RoleArn
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: CreationTime
  type: string
- description: ''
  name: TerminationDate
  type: string
- description: ''
  name: ProgressSummary
  type: object
- description: ''
  name: FailureReasons
  type: array
- description: ''
  name: Report
  type: object
- description: ''
  name: ConfirmationRequired
  type: boolean
- description: ''
  name: StatusUpdateReason
  type: string
- description: ''
  name: SuspendedDate
  type: string
- description: ''
  name: SuspendedCause
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-control-job-descriptor-schema.json
slug: amazon-s3-control-job-descriptor
source_filename: amazon-s3-control-job-descriptor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobDescriptor\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"Operation\": {\n      \"type\": \"object\"\n    },\n    \"Manifest\": {\n      \"type\": \"object\"\n    },\n    \"Priority\": {\n      \"type\": \"integer\"\n    },\n    \"RoleArn\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\"\n    },\n    \"TerminationDate\": {\n      \"type\": \"string\"\n    },\n    \"ProgressSummary\": {\n      \"type\": \"object\"\n    },\n    \"FailureReasons\": {\n      \"type\": \"array\"\n    },\n    \"Report\": {\n      \"type\": \"object\"\n    },\n    \"ConfirmationRequired\": {\n      \"type\": \"boolean\"\n    },\n    \"StatusUpdateReason\": {\n      \"type\": \"string\"\n    },\n\
  \    \"SuspendedDate\": {\n      \"type\": \"string\"\n    },\n    \"SuspendedCause\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-control-job-descriptor-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: JobDescriptor
---
