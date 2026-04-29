---
description: ''
layout: schema
name: StackResourceDrift
properties_list:
- description: ''
  name: StackId
  type: string
- description: ''
  name: LogicalResourceId
  type: string
- description: ''
  name: PhysicalResourceId
  type: string
- description: ''
  name: PhysicalResourceIdContext
  type: array
- description: ''
  name: ResourceType
  type: string
- description: A JSON string of the expected property values as defined in the template.
  name: ExpectedProperties
  type: string
- description: A JSON string of the actual property values of the resource.
  name: ActualProperties
  type: string
- description: ''
  name: PropertyDifferences
  type: array
- description: ''
  name: StackResourceDriftStatus
  type: string
- description: ''
  name: Timestamp
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-resource-drift-schema.json
slug: cloudformation-stack-resource-drift
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackResourceDrift\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackId\": {\n      \"type\": \"string\"\n    },\n    \"LogicalResourceId\": {\n      \"type\": \"string\"\n    },\n    \"PhysicalResourceId\": {\n      \"type\": \"string\"\n    },\n    \"PhysicalResourceIdContext\": {\n      \"type\": \"array\"\n    },\n    \"ResourceType\": {\n      \"type\": \"string\"\n    },\n    \"ExpectedProperties\": {\n      \"type\": \"string\",\n      \"description\": \"A JSON string of the expected property values as defined in the template.\"\n    },\n    \"ActualProperties\": {\n      \"type\": \"string\",\n      \"description\": \"A JSON string of the actual property values of the resource.\"\n    },\n    \"PropertyDifferences\": {\n      \"type\": \"array\"\n    },\n    \"StackResourceDriftStatus\": {\n      \"type\": \"string\"\n    },\n    \"Timestamp\": {\n      \"type\": \"string\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-resource-drift-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: StackResourceDrift
---
