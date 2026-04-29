---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: Error
  type: object
- description: ''
  name: RequestId
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-error-response-schema.json
slug: cloudformation-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Error\": {\n      \"type\": \"object\"\n    },\n    \"RequestId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-error-response-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: ErrorResponse
---
