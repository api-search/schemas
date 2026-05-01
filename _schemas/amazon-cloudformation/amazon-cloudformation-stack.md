---
description: Schema representing an Amazon CloudFormation stack, which is a collection of AWS resources that you can manage as a single unit.
layout: schema
name: Amazon CloudFormation Stack
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
- description: A list of Parameter structures that specify input parameters for the stack.
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
- description: Boolean to enable or disable rollback on stack creation failures.
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
- description: The Amazon Resource Name (ARN) of an IAM role that CloudFormation assumes to create the stack.
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
- description: A list of stack resources.
  name: Resources
  type: array
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/amazon-cloudformation-stack-schema.json
slug: amazon-cloudformation-stack
source_filename: amazon-cloudformation-stack-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://example.com/schemas/amazon-cloudformation-stack.json\",\n  \"title\": \"Amazon CloudFormation Stack\",\n  \"description\": \"Schema representing an Amazon CloudFormation stack, which is a collection of AWS resources that you can manage as a single unit.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"StackName\",\n    \"StackStatus\",\n    \"CreationTime\"\n  ],\n  \"properties\": {\n    \"StackId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the stack.\",\n      \"pattern\": \"^arn:aws:cloudformation:[a-z0-9-]+:[0-9]{12}:stack/.+/.+$\"\n    },\n    \"StackName\": {\n      \"type\": \"string\",\n      \"description\": \"The name associated with the stack.\",\n      \"minLength\": 1,\n      \"maxLength\": 128,\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9-]*$\"\n    },\n    \"ChangeSetId\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ unique ID of the change set.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A user-defined description associated with the stack.\",\n      \"maxLength\": 1024\n    },\n    \"Parameters\": {\n      \"type\": \"array\",\n      \"description\": \"A list of Parameter structures that specify input parameters for the stack.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Parameter\"\n      }\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time at which the stack was created.\"\n    },\n    \"DeletionTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the stack was deleted.\"\n    },\n    \"LastUpdatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the stack was last updated.\"\n    },\n    \"RollbackConfiguration\": {\n      \"$ref\": \"#/$defs/RollbackConfiguration\"\
  \n    },\n    \"StackStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the stack.\",\n      \"enum\": [\n        \"CREATE_IN_PROGRESS\",\n        \"CREATE_FAILED\",\n        \"CREATE_COMPLETE\",\n        \"ROLLBACK_IN_PROGRESS\",\n        \"ROLLBACK_FAILED\",\n        \"ROLLBACK_COMPLETE\",\n        \"DELETE_IN_PROGRESS\",\n        \"DELETE_FAILED\",\n        \"DELETE_COMPLETE\",\n        \"UPDATE_IN_PROGRESS\",\n        \"UPDATE_COMPLETE_CLEANUP_IN_PROGRESS\",\n        \"UPDATE_COMPLETE\",\n        \"UPDATE_FAILED\",\n        \"UPDATE_ROLLBACK_IN_PROGRESS\",\n        \"UPDATE_ROLLBACK_FAILED\",\n        \"UPDATE_ROLLBACK_COMPLETE_CLEANUP_IN_PROGRESS\",\n        \"UPDATE_ROLLBACK_COMPLETE\",\n        \"REVIEW_IN_PROGRESS\",\n        \"IMPORT_IN_PROGRESS\",\n        \"IMPORT_COMPLETE\",\n        \"IMPORT_ROLLBACK_IN_PROGRESS\",\n        \"IMPORT_ROLLBACK_FAILED\",\n        \"IMPORT_ROLLBACK_COMPLETE\"\n      ]\n    },\n    \"StackStatusReason\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"Success or failure message associated with the stack status.\"\n    },\n    \"DisableRollback\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean to enable or disable rollback on stack creation failures.\",\n      \"default\": false\n    },\n    \"NotificationARNs\": {\n      \"type\": \"array\",\n      \"description\": \"Amazon SNS topic ARNs to which stack related events are published.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^arn:aws:sns:[a-z0-9-]+:[0-9]{12}:.+$\"\n      },\n      \"maxItems\": 5\n    },\n    \"TimeoutInMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of time within which stack creation should complete.\",\n      \"minimum\": 1\n    },\n    \"Capabilities\": {\n      \"type\": \"array\",\n      \"description\": \"The capabilities allowed in the stack.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n   \
  \       \"CAPABILITY_IAM\",\n          \"CAPABILITY_NAMED_IAM\",\n          \"CAPABILITY_AUTO_EXPAND\"\n        ]\n      }\n    },\n    \"Outputs\": {\n      \"type\": \"array\",\n      \"description\": \"A list of output structures.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Output\"\n      }\n    },\n    \"RoleARN\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of an IAM role that CloudFormation assumes to create the stack.\",\n      \"pattern\": \"^arn:aws:iam::[0-9]{12}:role/.+$\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list of tags associated with the stack.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      },\n      \"maxItems\": 50\n    },\n    \"EnableTerminationProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether termination protection is enabled for the stack.\",\n      \"default\": false\n    },\n    \"DriftInformation\": {\n      \"$ref\": \"\
  #/$defs/StackDriftInformation\"\n    },\n    \"Resources\": {\n      \"type\": \"array\",\n      \"description\": \"A list of stack resources.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/StackResource\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Parameter\": {\n      \"type\": \"object\",\n      \"description\": \"A CloudFormation stack parameter.\",\n      \"properties\": {\n        \"ParameterKey\": {\n          \"type\": \"string\",\n          \"description\": \"The key associated with the parameter.\"\n        },\n        \"ParameterValue\": {\n          \"type\": \"string\",\n          \"description\": \"The input value associated with the parameter.\"\n        },\n        \"UsePreviousValue\": {\n          \"type\": \"boolean\",\n          \"description\": \"During a stack update, use the existing parameter value.\"\n        },\n        \"ResolvedValue\": {\n          \"type\": \"string\",\n          \"description\": \"Read-only. The value that corresponds to a SSM parameter\
  \ key.\"\n        }\n      },\n      \"required\": [\n        \"ParameterKey\"\n      ]\n    },\n    \"Output\": {\n      \"type\": \"object\",\n      \"description\": \"A CloudFormation stack output.\",\n      \"properties\": {\n        \"OutputKey\": {\n          \"type\": \"string\",\n          \"description\": \"The key associated with the output.\"\n        },\n        \"OutputValue\": {\n          \"type\": \"string\",\n          \"description\": \"The value associated with the output.\"\n        },\n        \"Description\": {\n          \"type\": \"string\",\n          \"description\": \"User defined description associated with the output.\"\n        },\n        \"ExportName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the export associated with the output.\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value pair tag.\",\n      \"required\": [\n        \"Key\",\n        \"Value\"\n  \
  \    ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"description\": \"The tag key.\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"description\": \"The tag value.\",\n          \"minLength\": 0,\n          \"maxLength\": 256\n        }\n      }\n    },\n    \"RollbackConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Structure containing the rollback triggers for CloudFormation to monitor during stack creation and updating operations.\",\n      \"properties\": {\n        \"RollbackTriggers\": {\n          \"type\": \"array\",\n          \"description\": \"The triggers to monitor during stack creation or update actions.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"Arn\",\n              \"Type\"\n            ],\n            \"properties\": {\n              \"Arn\":\
  \ {\n                \"type\": \"string\",\n                \"description\": \"The Amazon Resource Name (ARN) of the rollback trigger.\"\n              },\n              \"Type\": {\n                \"type\": \"string\",\n                \"description\": \"The resource type of the rollback trigger.\"\n              }\n            }\n          },\n          \"maxItems\": 5\n        },\n        \"MonitoringTimeInMinutes\": {\n          \"type\": \"integer\",\n          \"description\": \"The amount of time to monitor during rollback.\",\n          \"minimum\": 0,\n          \"maximum\": 180\n        }\n      }\n    },\n    \"StackDriftInformation\": {\n      \"type\": \"object\",\n      \"description\": \"Contains information about whether the stack drift detection has been performed and the status.\",\n      \"required\": [\n        \"StackDriftStatus\"\n      ],\n      \"properties\": {\n        \"StackDriftStatus\": {\n          \"type\": \"string\",\n          \"description\": \"Status\
  \ of the drift detection operation.\",\n          \"enum\": [\n            \"DRIFTED\",\n            \"IN_SYNC\",\n            \"UNKNOWN\",\n            \"NOT_CHECKED\"\n          ]\n        },\n        \"LastCheckTimestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Most recent time when a drift detection operation was initiated.\"\n        }\n      }\n    },\n    \"StackResource\": {\n      \"type\": \"object\",\n      \"description\": \"A resource that is part of a CloudFormation stack.\",\n      \"required\": [\n        \"LogicalResourceId\",\n        \"ResourceType\",\n        \"ResourceStatus\",\n        \"Timestamp\"\n      ],\n      \"properties\": {\n        \"StackName\": {\n          \"type\": \"string\",\n          \"description\": \"The name associated with the stack.\"\n        },\n        \"StackId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the stack.\"\n        },\n\
  \        \"LogicalResourceId\": {\n          \"type\": \"string\",\n          \"description\": \"The logical name of the resource specified in the template.\"\n        },\n        \"PhysicalResourceId\": {\n          \"type\": \"string\",\n          \"description\": \"The name or unique identifier that corresponds to a physical instance ID.\"\n        },\n        \"ResourceType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of resource (e.g., AWS::EC2::Instance).\"\n        },\n        \"Timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Time the status was updated.\"\n        },\n        \"ResourceStatus\": {\n          \"type\": \"string\",\n          \"description\": \"Current status of the resource.\",\n          \"enum\": [\n            \"CREATE_IN_PROGRESS\",\n            \"CREATE_FAILED\",\n            \"CREATE_COMPLETE\",\n            \"DELETE_IN_PROGRESS\",\n            \"DELETE_FAILED\"\
  ,\n            \"DELETE_COMPLETE\",\n            \"DELETE_SKIPPED\",\n            \"UPDATE_IN_PROGRESS\",\n            \"UPDATE_FAILED\",\n            \"UPDATE_COMPLETE\",\n            \"IMPORT_FAILED\",\n            \"IMPORT_COMPLETE\",\n            \"IMPORT_IN_PROGRESS\",\n            \"IMPORT_ROLLBACK_IN_PROGRESS\",\n            \"IMPORT_ROLLBACK_FAILED\",\n            \"IMPORT_ROLLBACK_COMPLETE\"\n          ]\n        },\n        \"ResourceStatusReason\": {\n          \"type\": \"string\",\n          \"description\": \"Success or failure message associated with the resource.\"\n        },\n        \"Description\": {\n          \"type\": \"string\",\n          \"description\": \"User defined description associated with the resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/amazon-cloudformation-stack-schema.json
tags:
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: Amazon CloudFormation Stack
---
