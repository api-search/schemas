---
description: Represents an AWS CloudFormation change set. A change set allows you to preview the changes CloudFormation will make to your stack before executing them. You can create a change set, review the proposed changes, and then choose to execute or delete it.
layout: schema
name: AWS CloudFormation Change Set
properties_list:
- description: The ARN of the change set.
  name: ChangeSetId
  type: string
- description: The name of the change set.
  name: ChangeSetName
  type: string
- description: The ID of the stack associated with the change set.
  name: StackId
  type: string
- description: The name of the stack associated with the change set.
  name: StackName
  type: string
- description: Information about the change set.
  name: Description
  type:
  - string
  - 'null'
- description: A list of parameter values for the change set.
  name: Parameters
  type: array
- description: The start time when the change set was created.
  name: CreationTime
  type: string
- description: The execution status of the change set.
  name: ExecutionStatus
  type: string
- description: The current status of the change set.
  name: Status
  type: string
- description: A description of the change set's status, such as why the change set failed.
  name: StatusReason
  type:
  - string
  - 'null'
- description: The ARNs of the Amazon SNS topics associated with the change set.
  name: NotificationARNs
  type: array
- description: ''
  name: RollbackConfiguration
  type: object
- description: The capabilities that are allowed in the change set.
  name: Capabilities
  type: array
- description: Tags associated with the change set.
  name: Tags
  type: array
- description: A list of structures that describe the resources and the actions that CloudFormation will perform.
  name: Changes
  type: array
- description: Whether the change set includes changes to nested stacks.
  name: IncludeNestedStacks
  type: boolean
- description: Whether the change set imports resources that already exist.
  name: ImportExistingResources
  type: boolean
- description: The parent change set ID for nested stack change sets.
  name: ParentChangeSetId
  type:
  - string
  - 'null'
- description: The root change set ID for nested stack change sets.
  name: RootChangeSetId
  type:
  - string
  - 'null'
- description: The type of change set operation.
  name: ChangeSetType
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/change-set.json
slug: change-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api.aws/cloudformation/change-set.json\",\n  \"title\": \"AWS CloudFormation Change Set\",\n  \"description\": \"Represents an AWS CloudFormation change set. A change set allows you to preview the changes CloudFormation will make to your stack before executing them. You can create a change set, review the proposed changes, and then choose to execute or delete it.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeSetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the change set.\",\n      \"pattern\": \"^arn:[-a-zA-Z0-9:/]*$\",\n      \"examples\": [\n        \"arn:aws:cloudformation:us-east-1:123456789012:changeSet/MyChangeSet/a1b2c3d4-5678-90ab-cdef-example11111\"\n      ]\n    },\n    \"ChangeSetName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the change set.\",\n      \"minLength\": 1,\n      \"maxLength\": 128,\n\
  \      \"pattern\": \"^[a-zA-Z][-a-zA-Z0-9]*$\"\n    },\n    \"StackId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the stack associated with the change set.\"\n    },\n    \"StackName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the stack associated with the change set.\"\n    },\n    \"Description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Information about the change set.\",\n      \"minLength\": 1,\n      \"maxLength\": 1024\n    },\n    \"Parameters\": {\n      \"type\": \"array\",\n      \"description\": \"A list of parameter values for the change set.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Parameter\"\n      }\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The start time when the change set was created.\"\n    },\n    \"ExecutionStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The execution status\
  \ of the change set.\",\n      \"enum\": [\n        \"UNAVAILABLE\",\n        \"AVAILABLE\",\n        \"EXECUTE_IN_PROGRESS\",\n        \"EXECUTE_COMPLETE\",\n        \"EXECUTE_FAILED\",\n        \"OBSOLETE\"\n      ]\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the change set.\",\n      \"enum\": [\n        \"CREATE_PENDING\",\n        \"CREATE_IN_PROGRESS\",\n        \"CREATE_COMPLETE\",\n        \"DELETE_PENDING\",\n        \"DELETE_IN_PROGRESS\",\n        \"DELETE_COMPLETE\",\n        \"DELETE_FAILED\",\n        \"FAILED\"\n      ]\n    },\n    \"StatusReason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A description of the change set's status, such as why the change set failed.\"\n    },\n    \"NotificationARNs\": {\n      \"type\": \"array\",\n      \"description\": \"The ARNs of the Amazon SNS topics associated with the change set.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n\
  \      \"maxItems\": 5\n    },\n    \"RollbackConfiguration\": {\n      \"$ref\": \"#/$defs/RollbackConfiguration\"\n    },\n    \"Capabilities\": {\n      \"type\": \"array\",\n      \"description\": \"The capabilities that are allowed in the change set.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"CAPABILITY_IAM\",\n          \"CAPABILITY_NAMED_IAM\",\n          \"CAPABILITY_AUTO_EXPAND\"\n        ]\n      }\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the change set.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      },\n      \"maxItems\": 50\n    },\n    \"Changes\": {\n      \"type\": \"array\",\n      \"description\": \"A list of structures that describe the resources and the actions that CloudFormation will perform.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Change\"\n      }\n    },\n    \"IncludeNestedStacks\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the change set includes changes to nested stacks.\"\n    },\n    \"ImportExistingResources\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the change set imports resources that already exist.\"\n    },\n    \"ParentChangeSetId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The parent change set ID for nested stack change sets.\"\n    },\n    \"RootChangeSetId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The root change set ID for nested stack change sets.\"\n    },\n    \"ChangeSetType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of change set operation.\",\n      \"enum\": [\n        \"CREATE\",\n        \"UPDATE\",\n        \"IMPORT\"\n      ]\n    }\n  },\n  \"$defs\": {\n    \"Parameter\": {\n      \"type\": \"object\",\n      \"description\": \"A parameter value for the change set.\",\n      \"properties\": {\n        \"ParameterKey\": {\n          \"type\": \"string\",\n \
  \         \"description\": \"The key associated with the parameter.\"\n        },\n        \"ParameterValue\": {\n          \"type\": \"string\",\n          \"description\": \"The input value associated with the parameter.\"\n        },\n        \"UsePreviousValue\": {\n          \"type\": \"boolean\",\n          \"description\": \"During a stack update, use the existing parameter value.\"\n        },\n        \"ResolvedValue\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Read-only. The value that corresponds to an SSM parameter key.\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"Key\",\n        \"Value\"\n      ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"minLength\": 0,\n          \"maxLength\": 256\n        }\n      }\n\
  \    },\n    \"RollbackConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"RollbackTriggers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"Arn\",\n              \"Type\"\n            ],\n            \"properties\": {\n              \"Arn\": {\n                \"type\": \"string\"\n              },\n              \"Type\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"maxItems\": 5\n        },\n        \"MonitoringTimeInMinutes\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 180\n        }\n      }\n    },\n    \"Change\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a change to a resource within a change set.\",\n      \"properties\": {\n        \"Type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of entity that CloudFormation\
  \ changes.\",\n          \"enum\": [\n            \"Resource\"\n          ]\n        },\n        \"ResourceChange\": {\n          \"$ref\": \"#/$defs/ResourceChange\"\n        }\n      }\n    },\n    \"ResourceChange\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the resource and the action that CloudFormation will perform on it.\",\n      \"properties\": {\n        \"Action\": {\n          \"type\": \"string\",\n          \"description\": \"The action that CloudFormation takes on the resource.\",\n          \"enum\": [\n            \"Add\",\n            \"Modify\",\n            \"Remove\",\n            \"Import\",\n            \"Dynamic\"\n          ]\n        },\n        \"LogicalResourceId\": {\n          \"type\": \"string\",\n          \"description\": \"The resource's logical ID in the template.\"\n        },\n        \"PhysicalResourceId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The resource's physical ID. Null for resources\
  \ being added.\"\n        },\n        \"ResourceType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of CloudFormation resource.\"\n        },\n        \"Replacement\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Whether the change requires the resource to be replaced.\",\n          \"enum\": [\n            \"True\",\n            \"False\",\n            \"Conditional\",\n            null\n          ]\n        },\n        \"Scope\": {\n          \"type\": \"array\",\n          \"description\": \"The properties or attributes whose changes triggered this resource change.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"Properties\",\n              \"Metadata\",\n              \"CreationPolicy\",\n              \"UpdatePolicy\",\n              \"DeletionPolicy\",\n              \"UpdateReplacePolicy\",\n              \"Tags\"\n            ]\n          }\n        },\n       \
  \ \"Details\": {\n          \"type\": \"array\",\n          \"description\": \"Details about the changes to the resource.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ResourceChangeDetail\"\n          }\n        }\n      }\n    },\n    \"ResourceChangeDetail\": {\n      \"type\": \"object\",\n      \"description\": \"Detailed information about a resource change.\",\n      \"properties\": {\n        \"Target\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Attribute\": {\n              \"type\": \"string\",\n              \"description\": \"The attribute that changed.\",\n              \"enum\": [\n                \"Properties\",\n                \"Metadata\",\n                \"CreationPolicy\",\n                \"UpdatePolicy\",\n                \"DeletionPolicy\",\n                \"UpdateReplacePolicy\",\n                \"Tags\"\n              ]\n            },\n            \"Name\": {\n              \"type\": [\"string\", \"null\"],\n\
  \              \"description\": \"The property name if the attribute is Properties.\"\n            },\n            \"RequiresRecreation\": {\n              \"type\": \"string\",\n              \"description\": \"Whether the change requires replacement.\",\n              \"enum\": [\n                \"Never\",\n                \"Conditionally\",\n                \"Always\"\n              ]\n            }\n          }\n        },\n        \"Evaluation\": {\n          \"type\": \"string\",\n          \"description\": \"Whether CloudFormation can determine the target value.\",\n          \"enum\": [\n            \"Static\",\n            \"Dynamic\"\n          ]\n        },\n        \"ChangeSource\": {\n          \"type\": \"string\",\n          \"description\": \"The entity that made the change.\",\n          \"enum\": [\n            \"ResourceReference\",\n            \"ParameterReference\",\n            \"ResourceAttribute\",\n            \"DirectModification\",\n            \"Automatic\"\
  \n          ]\n        },\n        \"CausingEntity\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The identity of the entity that triggered this change.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/change-set.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: AWS CloudFormation Change Set
---
