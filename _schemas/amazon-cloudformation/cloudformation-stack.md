---
description: Stack schema
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
- description: A list of Parameter structures.
  name: Parameters
  type: array
- description: The time at which the stack was created.
  name: CreationTime
  type: string
- description: The time the stack was deleted.
  name: DeletionTime
  type: string
- description: The time the stack was last updated.
  name: LastUpdatedTime
  type: string
- description: ''
  name: RollbackConfiguration
  type: object
- description: Current status of the stack.
  name: StackStatus
  type: string
- description: Success or failure message associated with the stack status.
  name: StackStatusReason
  type: string
- description: Whether rollback on stack creation failures is disabled.
  name: DisableRollback
  type: boolean
- description: Amazon SNS topic ARNs to which stack related events are published.
  name: NotificationARNs
  type: array
- description: The amount of time within which stack creation should complete.
  name: TimeoutInMinutes
  type: integer
- description: The capabilities allowed in the stack.
  name: Capabilities
  type: array
- description: A list of output structures.
  name: Outputs
  type: array
- description: The Amazon Resource Name (ARN) of an IAM role.
  name: RoleARN
  type: string
- description: A list of tags associated with the stack.
  name: Tags
  type: array
- description: Whether termination protection is enabled for the stack.
  name: EnableTerminationProtection
  type: boolean
- description: ''
  name: DriftInformation
  type: object
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-stack-schema.json
slug: cloudformation-stack
source_filename: cloudformation-stack-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-stack-schema.json\",\n  \"title\": \"Stack\",\n  \"description\": \"Stack schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the stack.\"\n    },\n    \"StackName\": {\n      \"type\": \"string\",\n      \"description\": \"The name associated with the stack.\"\n    },\n    \"ChangeSetId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the change set.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A user-defined description associated with the stack.\"\n    },\n    \"Parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Parameter\"\n      },\n      \"description\"\
  : \"A list of Parameter structures.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time at which the stack was created.\"\n    },\n    \"DeletionTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the stack was deleted.\"\n    },\n    \"LastUpdatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the stack was last updated.\"\n    },\n    \"RollbackConfiguration\": {\n      \"$ref\": \"#/components/schemas/RollbackConfiguration\"\n    },\n    \"StackStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the stack.\",\n      \"enum\": [\n        \"CREATE_IN_PROGRESS\",\n        \"CREATE_FAILED\",\n        \"CREATE_COMPLETE\",\n        \"ROLLBACK_IN_PROGRESS\",\n        \"ROLLBACK_FAILED\",\n        \"ROLLBACK_COMPLETE\",\n        \"DELETE_IN_PROGRESS\",\n        \"\
  DELETE_FAILED\",\n        \"DELETE_COMPLETE\",\n        \"UPDATE_IN_PROGRESS\",\n        \"UPDATE_COMPLETE_CLEANUP_IN_PROGRESS\",\n        \"UPDATE_COMPLETE\",\n        \"UPDATE_FAILED\",\n        \"UPDATE_ROLLBACK_IN_PROGRESS\",\n        \"UPDATE_ROLLBACK_FAILED\",\n        \"UPDATE_ROLLBACK_COMPLETE_CLEANUP_IN_PROGRESS\",\n        \"UPDATE_ROLLBACK_COMPLETE\",\n        \"REVIEW_IN_PROGRESS\",\n        \"IMPORT_IN_PROGRESS\",\n        \"IMPORT_COMPLETE\",\n        \"IMPORT_ROLLBACK_IN_PROGRESS\",\n        \"IMPORT_ROLLBACK_FAILED\",\n        \"IMPORT_ROLLBACK_COMPLETE\"\n      ]\n    },\n    \"StackStatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"Success or failure message associated with the stack status.\"\n    },\n    \"DisableRollback\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether rollback on stack creation failures is disabled.\"\n    },\n    \"NotificationARNs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"\
  string\"\n      },\n      \"description\": \"Amazon SNS topic ARNs to which stack related events are published.\"\n    },\n    \"TimeoutInMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of time within which stack creation should complete.\"\n    },\n    \"Capabilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"CAPABILITY_IAM\",\n          \"CAPABILITY_NAMED_IAM\",\n          \"CAPABILITY_AUTO_EXPAND\"\n        ]\n      },\n      \"description\": \"The capabilities allowed in the stack.\"\n    },\n    \"Outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Output\"\n      },\n      \"description\": \"A list of output structures.\"\n    },\n    \"RoleARN\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of an IAM role.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n\
  \        \"$ref\": \"#/components/schemas/Tag\"\n      },\n      \"description\": \"A list of tags associated with the stack.\"\n    },\n    \"EnableTerminationProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether termination protection is enabled for the stack.\"\n    },\n    \"DriftInformation\": {\n      \"$ref\": \"#/components/schemas/StackDriftInformation\"\n    }\n  },\n  \"required\": [\n    \"StackName\",\n    \"StackStatus\",\n    \"CreationTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-stack-schema.json
tags:
- AWS
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: Stack
---
