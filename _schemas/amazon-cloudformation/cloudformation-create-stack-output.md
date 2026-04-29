---
description: CreateStackOutput schema
layout: schema
name: CreateStackOutput
properties_list:
- description: Unique identifier of the stack.
  name: StackId
  type: string
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-create-stack-output-schema.json
slug: cloudformation-create-stack-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-create-stack-output-schema.json\",\n  \"title\": \"CreateStackOutput\",\n  \"description\": \"CreateStackOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the stack.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-create-stack-output-schema.json
tags:
- AWS
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: CreateStackOutput
---
