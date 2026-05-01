---
description: ''
layout: schema
name: StackResourceDriftInformation
properties_list:
- description: ''
  name: StackResourceDriftStatus
  type: string
- description: ''
  name: LastCheckTimestamp
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-resource-drift-information-schema.json
slug: cloudformation-stack-resource-drift-information
source_filename: cloudformation-stack-resource-drift-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackResourceDriftInformation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackResourceDriftStatus\": {\n      \"type\": \"string\"\n    },\n    \"LastCheckTimestamp\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-resource-drift-information-schema.json
tags:
- Automation
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: StackResourceDriftInformation
---
