---
description: ''
layout: schema
name: Stack
properties_list:
- description: Unique identifier of the stack.
  name: StackId
  type: string
- description: The name associated with the stack.
  name: StackName
  type: string
- description: The unique ID of the change set.
  name: ChangeSetId
  type: string
- description: A user-defined description associated with the stack.
  name: Description
  type: string
- description: The time the stack was created.
  name: CreationTime
  type: string
- description: The time the stack was deleted.
  name: DeletionTime
  type: string
- description: The time the stack was last updated.
  name: LastUpdatedTime
  type: string
- description: Explanation for the current stack status.
  name: StackStatusReason
  type: string
- description: Whether rollback on stack creation failures is disabled.
  name: DisableRollback
  type: boolean
- description: Amazon SNS topic ARNs for stack event notifications.
  name: NotificationARNs
  type: array
- description: Time allowed for stack creation before failure.
  name: TimeoutInMinutes
  type: integer
- description: The capabilities allowed in the stack.
  name: Capabilities
  type: array
- description: A list of output structures.
  name: Outputs
  type: array
- description: The IAM role ARN used by CloudFormation.
  name: RoleARN
  type: string
- description: Tags associated with the stack.
  name: Tags
  type: array
- description: Whether termination protection is enabled.
  name: EnableTerminationProtection
  type: boolean
- description: A list of parameter structures.
  name: Parameters
  type: array
- description: For nested stacks, the stack ID of the direct parent.
  name: ParentId
  type: string
- description: For nested stacks, the stack ID of the top-level stack.
  name: RootId
  type: string
- description: ''
  name: DeletionMode
  type: string
- description: ''
  name: DetailedStatus
  type: string
- description: ''
  name: RetainExceptOnCreate
  type: boolean
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-schema.json
slug: cloudformation-stack
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Stack\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the stack.\"\n    },\n    \"StackName\": {\n      \"type\": \"string\",\n      \"description\": \"The name associated with the stack.\"\n    },\n    \"ChangeSetId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the change set.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A user-defined description associated with the stack.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the stack was created.\"\n    },\n    \"DeletionTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the stack was deleted.\"\n    },\n    \"LastUpdatedTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the stack\
  \ was last updated.\"\n    },\n    \"StackStatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"Explanation for the current stack status.\"\n    },\n    \"DisableRollback\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether rollback on stack creation failures is disabled.\"\n    },\n    \"NotificationARNs\": {\n      \"type\": \"array\",\n      \"description\": \"Amazon SNS topic ARNs for stack event notifications.\"\n    },\n    \"TimeoutInMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Time allowed for stack creation before failure.\"\n    },\n    \"Capabilities\": {\n      \"type\": \"array\",\n      \"description\": \"The capabilities allowed in the stack.\"\n    },\n    \"Outputs\": {\n      \"type\": \"array\",\n      \"description\": \"A list of output structures.\"\n    },\n    \"RoleARN\": {\n      \"type\": \"string\",\n      \"description\": \"The IAM role ARN used by CloudFormation.\"\n    },\n    \"Tags\": {\n      \"\
  type\": \"array\",\n      \"description\": \"Tags associated with the stack.\"\n    },\n    \"EnableTerminationProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether termination protection is enabled.\"\n    },\n    \"Parameters\": {\n      \"type\": \"array\",\n      \"description\": \"A list of parameter structures.\"\n    },\n    \"ParentId\": {\n      \"type\": \"string\",\n      \"description\": \"For nested stacks, the stack ID of the direct parent.\"\n    },\n    \"RootId\": {\n      \"type\": \"string\",\n      \"description\": \"For nested stacks, the stack ID of the top-level stack.\"\n    },\n    \"DeletionMode\": {\n      \"type\": \"string\"\n    },\n    \"DetailedStatus\": {\n      \"type\": \"string\"\n    },\n    \"RetainExceptOnCreate\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: Stack
---
