---
description: ''
layout: schema
name: StackEvent
properties_list:
- description: ''
  name: StackId
  type: string
- description: ''
  name: EventId
  type: string
- description: ''
  name: StackName
  type: string
- description: ''
  name: LogicalResourceId
  type: string
- description: ''
  name: PhysicalResourceId
  type: string
- description: ''
  name: ResourceType
  type: string
- description: ''
  name: Timestamp
  type: string
- description: ''
  name: ResourceStatus
  type: string
- description: ''
  name: ResourceStatusReason
  type: string
- description: ''
  name: ResourceProperties
  type: string
- description: ''
  name: ClientRequestToken
  type: string
- description: ''
  name: HookType
  type: string
- description: ''
  name: HookStatus
  type: string
- description: ''
  name: HookStatusReason
  type: string
- description: ''
  name: HookInvocationPoint
  type: string
- description: ''
  name: HookFailureMode
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-event-schema.json
slug: cloudformation-stack-event
source_filename: cloudformation-stack-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackEvent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackId\": {\n      \"type\": \"string\"\n    },\n    \"EventId\": {\n      \"type\": \"string\"\n    },\n    \"StackName\": {\n      \"type\": \"string\"\n    },\n    \"LogicalResourceId\": {\n      \"type\": \"string\"\n    },\n    \"PhysicalResourceId\": {\n      \"type\": \"string\"\n    },\n    \"ResourceType\": {\n      \"type\": \"string\"\n    },\n    \"Timestamp\": {\n      \"type\": \"string\"\n    },\n    \"ResourceStatus\": {\n      \"type\": \"string\"\n    },\n    \"ResourceStatusReason\": {\n      \"type\": \"string\"\n    },\n    \"ResourceProperties\": {\n      \"type\": \"string\"\n    },\n    \"ClientRequestToken\": {\n      \"type\": \"string\"\n    },\n    \"HookType\": {\n      \"type\": \"string\"\n    },\n    \"HookStatus\": {\n      \"type\": \"string\"\n    },\n    \"HookStatusReason\": {\n      \"type\"\
  : \"string\"\n    },\n    \"HookInvocationPoint\": {\n      \"type\": \"string\"\n    },\n    \"HookFailureMode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-event-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: StackEvent
---
