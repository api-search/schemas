---
description: Represents an AWS CloudFormation stack, which is a collection of AWS resources that you can manage as a single unit. A stack is created from a CloudFormation template and provisions the defined resources in the correct order based on dependency relationships.
layout: schema
name: AWS CloudFormation Stack
properties_list:
- description: Unique identifier of the stack, formatted as an Amazon Resource Name (ARN).
  name: StackId
  type: string
- description: The name associated with the stack. Must be unique within a region.
  name: StackName
  type: string
- description: The unique ID of the change set associated with this stack.
  name: ChangeSetId
  type: string
- description: A user-defined description associated with the stack.
  name: Description
  type:
  - string
  - 'null'
- description: The time at which the stack was created.
  name: CreationTime
  type: string
- description: The time the stack was deleted.
  name: DeletionTime
  type:
  - string
  - 'null'
- description: The time the stack was last updated. This field is only returned if the stack has been updated at least once.
  name: LastUpdatedTime
  type:
  - string
  - 'null'
- description: Current status of the stack.
  name: StackStatus
  type: string
- description: Success or failure message associated with the stack status.
  name: StackStatusReason
  type:
  - string
  - 'null'
- description: Boolean to enable or disable rollback on stack creation failures.
  name: DisableRollback
  type: boolean
- description: Amazon SNS topic ARNs to which stack related events are published.
  name: NotificationARNs
  type: array
- description: The amount of time within which stack creation should complete.
  name: TimeoutInMinutes
  type:
  - integer
  - 'null'
- description: The capabilities allowed in the stack.
  name: Capabilities
  type: array
- description: A list of output structures containing stack outputs.
  name: Outputs
  type: array
- description: The Amazon Resource Name (ARN) of an IAM role that CloudFormation assumes to create the stack.
  name: RoleARN
  type:
  - string
  - 'null'
- description: A list of tags associated with this stack.
  name: Tags
  type: array
- description: Whether termination protection is enabled for the stack.
  name: EnableTerminationProtection
  type: boolean
- description: A list of parameter structures.
  name: Parameters
  type: array
- description: ''
  name: RollbackConfiguration
  type: object
- description: For nested stacks, the stack ID of the direct parent of this stack.
  name: ParentId
  type:
  - string
  - 'null'
- description: For nested stacks, the stack ID of the top-level stack to which this stack belongs.
  name: RootId
  type:
  - string
  - 'null'
- description: ''
  name: DriftInformation
  type: object
- description: Specifies the deletion mode for the stack.
  name: DeletionMode
  type: string
- description: The detailed status of the resource or stack.
  name: DetailedStatus
  type:
  - string
  - 'null'
- description: When true, newly created resources are deleted when the operation rolls back.
  name: RetainExceptOnCreate
  type: boolean
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/stack.json
slug: stack
source_filename: stack.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api.aws/cloudformation/stack.json\",\n  \"title\": \"AWS CloudFormation Stack\",\n  \"description\": \"Represents an AWS CloudFormation stack, which is a collection of AWS resources that you can manage as a single unit. A stack is created from a CloudFormation template and provisions the defined resources in the correct order based on dependency relationships.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"StackName\",\n    \"CreationTime\",\n    \"StackStatus\"\n  ],\n  \"properties\": {\n    \"StackId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the stack, formatted as an Amazon Resource Name (ARN).\",\n      \"examples\": [\n        \"arn:aws:cloudformation:us-east-1:123456789012:stack/MyStack/aaf549a0-a413-11df-adb3-5081b3858e83\"\n      ]\n    },\n    \"StackName\": {\n      \"type\": \"string\",\n      \"description\": \"The name\
  \ associated with the stack. Must be unique within a region.\",\n      \"maxLength\": 128,\n      \"pattern\": \"^[a-zA-Z][-a-zA-Z0-9]*$\",\n      \"examples\": [\n        \"MyProductionStack\"\n      ]\n    },\n    \"ChangeSetId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the change set associated with this stack.\"\n    },\n    \"Description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A user-defined description associated with the stack.\",\n      \"maxLength\": 1024\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time at which the stack was created.\"\n    },\n    \"DeletionTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The time the stack was deleted.\"\n    },\n    \"LastUpdatedTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The time the stack was last updated. This field is only returned if the stack has been updated at least once.\"\n    },\n    \"StackStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the stack.\",\n      \"enum\": [\n        \"CREATE_IN_PROGRESS\",\n        \"CREATE_FAILED\",\n        \"CREATE_COMPLETE\",\n        \"ROLLBACK_IN_PROGRESS\",\n        \"ROLLBACK_FAILED\",\n        \"ROLLBACK_COMPLETE\",\n        \"DELETE_IN_PROGRESS\",\n        \"DELETE_FAILED\",\n        \"DELETE_COMPLETE\",\n        \"UPDATE_IN_PROGRESS\",\n        \"UPDATE_COMPLETE_CLEANUP_IN_PROGRESS\",\n        \"UPDATE_COMPLETE\",\n        \"UPDATE_FAILED\",\n        \"UPDATE_ROLLBACK_IN_PROGRESS\",\n        \"UPDATE_ROLLBACK_FAILED\",\n        \"UPDATE_ROLLBACK_COMPLETE_CLEANUP_IN_PROGRESS\",\n        \"UPDATE_ROLLBACK_COMPLETE\",\n        \"REVIEW_IN_PROGRESS\",\n        \"IMPORT_IN_PROGRESS\",\n        \"IMPORT_COMPLETE\",\n        \"IMPORT_ROLLBACK_IN_PROGRESS\",\n        \"\
  IMPORT_ROLLBACK_FAILED\",\n        \"IMPORT_ROLLBACK_COMPLETE\"\n      ]\n    },\n    \"StackStatusReason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Success or failure message associated with the stack status.\"\n    },\n    \"DisableRollback\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean to enable or disable rollback on stack creation failures.\",\n      \"default\": false\n    },\n    \"NotificationARNs\": {\n      \"type\": \"array\",\n      \"description\": \"Amazon SNS topic ARNs to which stack related events are published.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"maxItems\": 5\n    },\n    \"TimeoutInMinutes\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The amount of time within which stack creation should complete.\",\n      \"minimum\": 1\n    },\n    \"Capabilities\": {\n      \"type\": \"array\",\n      \"description\": \"The capabilities allowed in the stack.\",\n   \
  \   \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"CAPABILITY_IAM\",\n          \"CAPABILITY_NAMED_IAM\",\n          \"CAPABILITY_AUTO_EXPAND\"\n        ]\n      }\n    },\n    \"Outputs\": {\n      \"type\": \"array\",\n      \"description\": \"A list of output structures containing stack outputs.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Output\"\n      }\n    },\n    \"RoleARN\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The Amazon Resource Name (ARN) of an IAM role that CloudFormation assumes to create the stack.\",\n      \"minLength\": 20,\n      \"maxLength\": 2048\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list of tags associated with this stack.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      },\n      \"maxItems\": 50\n    },\n    \"EnableTerminationProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether termination protection is enabled\
  \ for the stack.\",\n      \"default\": false\n    },\n    \"Parameters\": {\n      \"type\": \"array\",\n      \"description\": \"A list of parameter structures.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Parameter\"\n      }\n    },\n    \"RollbackConfiguration\": {\n      \"$ref\": \"#/$defs/RollbackConfiguration\"\n    },\n    \"ParentId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"For nested stacks, the stack ID of the direct parent of this stack.\"\n    },\n    \"RootId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"For nested stacks, the stack ID of the top-level stack to which this stack belongs.\"\n    },\n    \"DriftInformation\": {\n      \"$ref\": \"#/$defs/StackDriftInformation\"\n    },\n    \"DeletionMode\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the deletion mode for the stack.\",\n      \"enum\": [\n        \"STANDARD\",\n        \"FORCE_DELETE_STACK\"\n      ]\n    },\n    \"DetailedStatus\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The detailed status of the resource or stack.\",\n      \"enum\": [\n        \"CONFIGURATION_COMPLETE\",\n        \"VALIDATION_FAILED\",\n        null\n      ]\n    },\n    \"RetainExceptOnCreate\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, newly created resources are deleted when the operation rolls back.\",\n      \"default\": false\n    }\n  },\n  \"$defs\": {\n    \"Output\": {\n      \"type\": \"object\",\n      \"description\": \"An output value from a CloudFormation stack.\",\n      \"properties\": {\n        \"OutputKey\": {\n          \"type\": \"string\",\n          \"description\": \"The key associated with the output.\"\n        },\n        \"OutputValue\": {\n          \"type\": \"string\",\n          \"description\": \"The value associated with the output.\"\n        },\n        \"Description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"User-defined\
  \ description of the output.\"\n        },\n        \"ExportName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The name of the export associated with this output for cross-stack references.\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value pair used to tag the stack.\",\n      \"required\": [\n        \"Key\",\n        \"Value\"\n      ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"description\": \"The tag key.\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"description\": \"The tag value.\",\n          \"minLength\": 0,\n          \"maxLength\": 256\n        }\n      }\n    },\n    \"Parameter\": {\n      \"type\": \"object\",\n      \"description\": \"An input parameter for the stack.\",\n      \"properties\": {\n        \"ParameterKey\": {\n       \
  \   \"type\": \"string\",\n          \"description\": \"The key associated with the parameter.\"\n        },\n        \"ParameterValue\": {\n          \"type\": \"string\",\n          \"description\": \"The input value associated with the parameter.\"\n        },\n        \"UsePreviousValue\": {\n          \"type\": \"boolean\",\n          \"description\": \"During a stack update, use the existing parameter value.\"\n        },\n        \"ResolvedValue\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Read-only. The value that corresponds to an SSM parameter key.\"\n        }\n      }\n    },\n    \"RollbackConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Monitoring and rollback configuration for the stack.\",\n      \"properties\": {\n        \"RollbackTriggers\": {\n          \"type\": \"array\",\n          \"description\": \"The triggers to monitor during stack creation or update actions.\",\n          \"items\": {\n           \
  \ \"type\": \"object\",\n            \"required\": [\n              \"Arn\",\n              \"Type\"\n            ],\n            \"properties\": {\n              \"Arn\": {\n                \"type\": \"string\",\n                \"description\": \"The ARN of the rollback trigger (must be a CloudWatch alarm).\"\n              },\n              \"Type\": {\n                \"type\": \"string\",\n                \"description\": \"The resource type of the rollback trigger.\"\n              }\n            }\n          },\n          \"maxItems\": 5\n        },\n        \"MonitoringTimeInMinutes\": {\n          \"type\": \"integer\",\n          \"description\": \"The amount of time in minutes to monitor after stack deployment.\",\n          \"minimum\": 0,\n          \"maximum\": 180\n        }\n      }\n    },\n    \"StackDriftInformation\": {\n      \"type\": \"object\",\n      \"description\": \"Contains information about whether the stack's actual configuration differs from its expected\
  \ configuration.\",\n      \"required\": [\n        \"StackDriftStatus\"\n      ],\n      \"properties\": {\n        \"StackDriftStatus\": {\n          \"type\": \"string\",\n          \"description\": \"Status of the stack's actual configuration compared to its expected template configuration.\",\n          \"enum\": [\n            \"DRIFTED\",\n            \"IN_SYNC\",\n            \"UNKNOWN\",\n            \"NOT_CHECKED\"\n          ]\n        },\n        \"LastCheckTimestamp\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"Most recent time when a drift detection operation was initiated.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/stack.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: AWS CloudFormation Stack
---
