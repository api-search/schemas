---
description: ''
layout: schema
name: StackResource
properties_list:
- description: The name of the stack.
  name: StackName
  type: string
- description: Unique identifier of the stack.
  name: StackId
  type: string
- description: The logical name of the resource specified in the template.
  name: LogicalResourceId
  type: string
- description: The name or unique identifier of the physical resource.
  name: PhysicalResourceId
  type: string
- description: Type of AWS resource.
  name: ResourceType
  type: string
- description: Time the status was updated.
  name: Timestamp
  type: string
- description: Current status of the resource.
  name: ResourceStatus
  type: string
- description: Message associated with the resource status.
  name: ResourceStatusReason
  type: string
- description: User-defined description.
  name: Description
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-resource-schema.json
slug: cloudformation-stack-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackResource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the stack.\"\n    },\n    \"StackId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the stack.\"\n    },\n    \"LogicalResourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The logical name of the resource specified in the template.\"\n    },\n    \"PhysicalResourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The name or unique identifier of the physical resource.\"\n    },\n    \"ResourceType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of AWS resource.\"\n    },\n    \"Timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Time the status was updated.\"\n    },\n    \"ResourceStatus\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Current status of the resource.\"\n    },\n    \"ResourceStatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"Message associated with the resource status.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined description.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-resource-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: StackResource
---
