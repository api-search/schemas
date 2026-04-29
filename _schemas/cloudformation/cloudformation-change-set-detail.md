---
description: ''
layout: schema
name: ChangeSetDetail
properties_list:
- description: ''
  name: ChangeSetName
  type: string
- description: ''
  name: ChangeSetId
  type: string
- description: ''
  name: StackId
  type: string
- description: ''
  name: StackName
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: Parameters
  type: array
- description: ''
  name: CreationTime
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
  name: NotificationARNs
  type: array
- description: ''
  name: Capabilities
  type: array
- description: ''
  name: Tags
  type: array
- description: ''
  name: Changes
  type: array
- description: ''
  name: IncludeNestedStacks
  type: boolean
- description: ''
  name: NextToken
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-change-set-detail-schema.json
slug: cloudformation-change-set-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChangeSetDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeSetName\": {\n      \"type\": \"string\"\n    },\n    \"ChangeSetId\": {\n      \"type\": \"string\"\n    },\n    \"StackId\": {\n      \"type\": \"string\"\n    },\n    \"StackName\": {\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"Parameters\": {\n      \"type\": \"array\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\"\n    },\n    \"ExecutionStatus\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\"\n    },\n    \"StatusReason\": {\n      \"type\": \"string\"\n    },\n    \"NotificationARNs\": {\n      \"type\": \"array\"\n    },\n    \"Capabilities\": {\n      \"type\": \"array\"\n    },\n    \"Tags\": {\n      \"type\": \"array\"\n    },\n    \"Changes\": {\n      \"type\": \"array\"\n    },\n    \"IncludeNestedStacks\"\
  : {\n      \"type\": \"boolean\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-change-set-detail-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: ChangeSetDetail
---
