---
description: A complete lifecycle policy definition for automating EBS snapshot or AMI management.
layout: schema
name: Lifecycle Policy
properties_list:
- description: The identifier of the lifecycle policy
  name: PolicyId
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: State
  type: string
- description: The ARN of the IAM role used by DLM
  name: ExecutionRoleArn
  type: string
- description: ''
  name: DateCreated
  type: string
- description: ''
  name: DateModified
  type: string
- description: ''
  name: PolicyDetails
  type: object
provider_name: Amazon Data Lifecycle Manager
provider_slug: amazon-data-lifecycle-manager
schema_file: json-schema/lifecycle-policy-schema.json
slug: lifecycle-policy
source_filename: lifecycle-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-lifecycle-manager/json-schema/lifecycle-policy-schema.json\",\n  \"title\": \"Lifecycle Policy\",\n  \"description\": \"A complete lifecycle policy definition for automating EBS snapshot or AMI management.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the lifecycle policy\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\",\n        \"ERROR\"\n      ]\n    },\n    \"ExecutionRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role used by DLM\"\n    },\n    \"DateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"DateModified\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\"\n    },\n    \"PolicyDetails\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-lifecycle-manager/refs/heads/main/json-schema/lifecycle-policy-schema.json
tags:
- AWS
- Backup
- EBS Snapshots
- Lifecycle Management
- Storage
- Automation
- Compliance
title: Lifecycle Policy
---
