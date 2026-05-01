---
description: CreateChangeSetOutput schema
layout: schema
name: CreateChangeSetOutput
properties_list:
- description: The ARN of the change set.
  name: Id
  type: string
- description: The unique ID of the stack.
  name: StackId
  type: string
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-create-change-set-output-schema.json
slug: cloudformation-create-change-set-output
source_filename: cloudformation-create-change-set-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-create-change-set-output-schema.json\",\n  \"title\": \"CreateChangeSetOutput\",\n  \"description\": \"CreateChangeSetOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the change set.\"\n    },\n    \"StackId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the stack.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-create-change-set-output-schema.json
tags:
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: CreateChangeSetOutput
---
