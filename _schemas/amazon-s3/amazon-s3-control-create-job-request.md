---
description: ''
layout: schema
name: CreateJobRequest
properties_list:
- description: The action that you want the job to perform on each object.
  name: Operation
  type: object
- description: Configuration parameters for the optional completion report for the job.
  name: Report
  type: object
- description: Configuration parameters for the manifest.
  name: Manifest
  type: object
- description: The numerical priority for this job.
  name: Priority
  type: integer
- description: The Amazon Resource Name (ARN) for the IAM role.
  name: RoleArn
  type: string
- description: A description for this job.
  name: Description
  type: string
- description: Indicates whether confirmation is required before Amazon S3 runs the job.
  name: ConfirmationRequired
  type: boolean
- description: ''
  name: Tags
  type: array
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-control-create-job-request-schema.json
slug: amazon-s3-control-create-job-request
source_filename: amazon-s3-control-create-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateJobRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Operation\": {\n      \"type\": \"object\",\n      \"description\": \"The action that you want the job to perform on each object.\"\n    },\n    \"Report\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration parameters for the optional completion report for the job.\"\n    },\n    \"Manifest\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration parameters for the manifest.\"\n    },\n    \"Priority\": {\n      \"type\": \"integer\",\n      \"description\": \"The numerical priority for this job.\"\n    },\n    \"RoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the IAM role.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A description for this job.\"\n    },\n    \"ConfirmationRequired\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether confirmation is required before Amazon S3 runs the job.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-control-create-job-request-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: CreateJobRequest
---
