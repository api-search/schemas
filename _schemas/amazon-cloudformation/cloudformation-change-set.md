---
description: ChangeSet schema
layout: schema
name: ChangeSet
properties_list:
- description: The ARN of the change set.
  name: ChangeSetId
  type: string
- description: The name of the change set.
  name: ChangeSetName
  type: string
- description: The ARN of the stack associated with the change set.
  name: StackId
  type: string
- description: The name of the stack associated with the change set.
  name: StackName
  type: string
- description: Information about the change set.
  name: Description
  type: string
- description: The execution status of the change set.
  name: ExecutionStatus
  type: string
- description: The current status of the change set.
  name: Status
  type: string
- description: A description of the current status of the change set.
  name: StatusReason
  type: string
- description: The start time when the change set was created.
  name: CreationTime
  type: string
- description: A list of structures that describe the resources and their changes.
  name: Changes
  type: array
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-change-set-schema.json
slug: cloudformation-change-set
source_filename: cloudformation-change-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-change-set-schema.json\",\n  \"title\": \"ChangeSet\",\n  \"description\": \"ChangeSet schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeSetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the change set.\"\n    },\n    \"ChangeSetName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the change set.\"\n    },\n    \"StackId\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the stack associated with the change set.\"\n    },\n    \"StackName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the stack associated with the change set.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Information about the change set.\"\n    },\n    \"ExecutionStatus\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"UNAVAILABLE\",\n        \"AVAILABLE\",\n        \"EXECUTE_IN_PROGRESS\",\n        \"EXECUTE_COMPLETE\",\n        \"EXECUTE_FAILED\",\n        \"OBSOLETE\"\n      ],\n      \"description\": \"The execution status of the change set.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATE_PENDING\",\n        \"CREATE_IN_PROGRESS\",\n        \"CREATE_COMPLETE\",\n        \"DELETE_FAILED\",\n        \"DELETE_COMPLETE\",\n        \"FAILED\"\n      ],\n      \"description\": \"The current status of the change set.\"\n    },\n    \"StatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the current status of the change set.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The start time when the change set was created.\"\n    },\n    \"Changes\": {\n      \"type\": \"array\",\n      \"\
  items\": {\n        \"$ref\": \"#/components/schemas/Change\"\n      },\n      \"description\": \"A list of structures that describe the resources and their changes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-change-set-schema.json
tags:
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: ChangeSet
---
