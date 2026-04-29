---
description: ''
layout: schema
name: StackDriftInformation
properties_list:
- description: ''
  name: StackDriftStatus
  type: string
- description: ''
  name: LastCheckTimestamp
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-drift-information-schema.json
slug: cloudformation-stack-drift-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackDriftInformation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackDriftStatus\": {\n      \"type\": \"string\"\n    },\n    \"LastCheckTimestamp\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-drift-information-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: StackDriftInformation
---
