---
description: StackResource schema
layout: schema
name: StackResource
properties_list:
- description: The name associated with the stack.
  name: StackName
  type: string
- description: Unique identifier of the stack.
  name: StackId
  type: string
- description: The logical name of the resource specified in the template.
  name: LogicalResourceId
  type: string
- description: The name or unique identifier of the resource.
  name: PhysicalResourceId
  type: string
- description: Type of resource (e.g., AWS::EC2::Instance).
  name: ResourceType
  type: string
- description: Time the status was updated.
  name: Timestamp
  type: string
- description: Current status of the resource.
  name: ResourceStatus
  type: string
- description: Success or failure message associated with the resource.
  name: ResourceStatusReason
  type: string
- description: User defined description associated with the resource.
  name: Description
  type: string
- description: ''
  name: DriftInformation
  type: object
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-stack-resource-schema.json
slug: cloudformation-stack-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-stack-resource-schema.json\",\n  \"title\": \"StackResource\",\n  \"description\": \"StackResource schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackName\": {\n      \"type\": \"string\",\n      \"description\": \"The name associated with the stack.\"\n    },\n    \"StackId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the stack.\"\n    },\n    \"LogicalResourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The logical name of the resource specified in the template.\"\n    },\n    \"PhysicalResourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The name or unique identifier of the resource.\"\n    },\n    \"ResourceType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of resource (e.g.,\
  \ AWS::EC2::Instance).\"\n    },\n    \"Timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time the status was updated.\"\n    },\n    \"ResourceStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATE_IN_PROGRESS\",\n        \"CREATE_FAILED\",\n        \"CREATE_COMPLETE\",\n        \"DELETE_IN_PROGRESS\",\n        \"DELETE_FAILED\",\n        \"DELETE_COMPLETE\",\n        \"DELETE_SKIPPED\",\n        \"UPDATE_IN_PROGRESS\",\n        \"UPDATE_FAILED\",\n        \"UPDATE_COMPLETE\",\n        \"IMPORT_FAILED\",\n        \"IMPORT_COMPLETE\",\n        \"IMPORT_IN_PROGRESS\",\n        \"IMPORT_ROLLBACK_IN_PROGRESS\",\n        \"IMPORT_ROLLBACK_FAILED\",\n        \"IMPORT_ROLLBACK_COMPLETE\"\n      ],\n      \"description\": \"Current status of the resource.\"\n    },\n    \"ResourceStatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"Success or failure message associated with the resource.\"\n    },\n\
  \    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"User defined description associated with the resource.\"\n    },\n    \"DriftInformation\": {\n      \"$ref\": \"#/components/schemas/StackResourceDriftInformation\"\n    }\n  },\n  \"required\": [\n    \"LogicalResourceId\",\n    \"ResourceType\",\n    \"ResourceStatus\",\n    \"Timestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-stack-resource-schema.json
tags:
- AWS
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: StackResource
---
