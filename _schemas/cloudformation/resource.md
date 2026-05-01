---
description: Represents a resource within an AWS CloudFormation stack. Each resource corresponds to a physical AWS service resource (such as an EC2 instance, S3 bucket, or Lambda function) that is provisioned and managed as part of the stack lifecycle.
layout: schema
name: AWS CloudFormation Stack Resource
properties_list:
- description: The name of the stack the resource belongs to.
  name: StackName
  type:
  - string
  - 'null'
- description: Unique identifier of the stack.
  name: StackId
  type:
  - string
  - 'null'
- description: The logical name of the resource as specified in the template.
  name: LogicalResourceId
  type: string
- description: The name or unique identifier that corresponds to a physical instance ID of the resource.
  name: PhysicalResourceId
  type:
  - string
  - 'null'
- description: The type of the resource (e.g. AWS::EC2::Instance, AWS::S3::Bucket).
  name: ResourceType
  type: string
- description: The time the status was updated.
  name: Timestamp
  type: string
- description: Current status of the resource.
  name: ResourceStatus
  type: string
- description: Success or failure message associated with the resource.
  name: ResourceStatusReason
  type:
  - string
  - 'null'
- description: User-defined description associated with the resource.
  name: Description
  type:
  - string
  - 'null'
- description: ''
  name: DriftInformation
  type: object
- description: ''
  name: ModuleInfo
  type: object
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/resource.json
slug: resource
source_filename: resource.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api.aws/cloudformation/resource.json\",\n  \"title\": \"AWS CloudFormation Stack Resource\",\n  \"description\": \"Represents a resource within an AWS CloudFormation stack. Each resource corresponds to a physical AWS service resource (such as an EC2 instance, S3 bucket, or Lambda function) that is provisioned and managed as part of the stack lifecycle.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"LogicalResourceId\",\n    \"ResourceType\",\n    \"ResourceStatus\",\n    \"Timestamp\"\n  ],\n  \"properties\": {\n    \"StackName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of the stack the resource belongs to.\"\n    },\n    \"StackId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Unique identifier of the stack.\"\n    },\n    \"LogicalResourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The logical\
  \ name of the resource as specified in the template.\"\n    },\n    \"PhysicalResourceId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name or unique identifier that corresponds to a physical instance ID of the resource.\"\n    },\n    \"ResourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource (e.g. AWS::EC2::Instance, AWS::S3::Bucket).\",\n      \"minLength\": 1,\n      \"maxLength\": 256,\n      \"examples\": [\n        \"AWS::EC2::Instance\",\n        \"AWS::S3::Bucket\",\n        \"AWS::Lambda::Function\",\n        \"AWS::IAM::Role\"\n      ]\n    },\n    \"Timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the status was updated.\"\n    },\n    \"ResourceStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the resource.\",\n      \"enum\": [\n        \"CREATE_IN_PROGRESS\",\n        \"CREATE_FAILED\",\n        \"CREATE_COMPLETE\"\
  ,\n        \"DELETE_IN_PROGRESS\",\n        \"DELETE_FAILED\",\n        \"DELETE_COMPLETE\",\n        \"UPDATE_IN_PROGRESS\",\n        \"UPDATE_FAILED\",\n        \"UPDATE_COMPLETE\",\n        \"IMPORT_FAILED\",\n        \"IMPORT_COMPLETE\",\n        \"IMPORT_IN_PROGRESS\",\n        \"IMPORT_ROLLBACK_IN_PROGRESS\",\n        \"IMPORT_ROLLBACK_FAILED\",\n        \"IMPORT_ROLLBACK_COMPLETE\",\n        \"ROLLBACK_IN_PROGRESS\",\n        \"ROLLBACK_COMPLETE\"\n      ]\n    },\n    \"ResourceStatusReason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Success or failure message associated with the resource.\"\n    },\n    \"Description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"User-defined description associated with the resource.\",\n      \"maxLength\": 1024\n    },\n    \"DriftInformation\": {\n      \"$ref\": \"#/$defs/StackResourceDriftInformation\"\n    },\n    \"ModuleInfo\": {\n      \"$ref\": \"#/$defs/ModuleInfo\"\n    }\n  },\n\
  \  \"$defs\": {\n    \"StackResourceDriftInformation\": {\n      \"type\": \"object\",\n      \"description\": \"Summarizes information about whether the resource's actual configuration differs from its expected configuration.\",\n      \"required\": [\n        \"StackResourceDriftStatus\"\n      ],\n      \"properties\": {\n        \"StackResourceDriftStatus\": {\n          \"type\": \"string\",\n          \"description\": \"Status of the resource's actual configuration compared to its expected configuration.\",\n          \"enum\": [\n            \"IN_SYNC\",\n            \"MODIFIED\",\n            \"DELETED\",\n            \"NOT_CHECKED\"\n          ]\n        },\n        \"LastCheckTimestamp\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"When CloudFormation last checked if the resource had drifted from its expected configuration.\"\n        }\n      }\n    },\n    \"ModuleInfo\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Contains information about the module from which the resource was created, if the resource was created from a module included in the stack template.\",\n      \"properties\": {\n        \"TypeHierarchy\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A concatenated list of the module type or types containing the resource.\"\n        },\n        \"LogicalIdHierarchy\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A concatenated list of the logical IDs of the module or modules containing the resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/resource.json
tags:
- Automation
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: AWS CloudFormation Stack Resource
---
