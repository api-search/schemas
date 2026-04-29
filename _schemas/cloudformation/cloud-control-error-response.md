---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: The error message.
  name: Message
  type: string
- description: The error code.
  name: Code
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloud-control-error-response-schema.json
slug: cloud-control-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Message\": {\n      \"type\": \"string\",\n      \"description\": \"The error message.\"\n    },\n    \"Code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloud-control-error-response-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: ErrorResponse
---
