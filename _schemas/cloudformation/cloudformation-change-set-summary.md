---
description: ''
layout: schema
name: ChangeSetSummary
properties_list:
- description: The ID of the stack with which the change set is associated.
  name: StackId
  type: string
- description: ''
  name: StackName
  type: string
- description: The ARN of the change set.
  name: ChangeSetId
  type: string
- description: ''
  name: ChangeSetName
  type: string
- description: ''
  name: ExecutionStatus
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: StatusReason
  type: string
- description: ''
  name: CreationTime
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: IncludeNestedStacks
  type: boolean
- description: ''
  name: ImportExistingResources
  type: boolean
- description: ''
  name: ParentChangeSetId
  type: string
- description: ''
  name: RootChangeSetId
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-change-set-summary-schema.json
slug: cloudformation-change-set-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChangeSetSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the stack with which the change set is associated.\"\n    },\n    \"StackName\": {\n      \"type\": \"string\"\n    },\n    \"ChangeSetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the change set.\"\n    },\n    \"ChangeSetName\": {\n      \"type\": \"string\"\n    },\n    \"ExecutionStatus\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\"\n    },\n    \"StatusReason\": {\n      \"type\": \"string\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"IncludeNestedStacks\": {\n      \"type\": \"boolean\"\n    },\n    \"ImportExistingResources\": {\n      \"type\": \"boolean\"\n    },\n    \"ParentChangeSetId\"\
  : {\n      \"type\": \"string\"\n    },\n    \"RootChangeSetId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-change-set-summary-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: ChangeSetSummary
---
