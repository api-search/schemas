---
description: ''
layout: schema
name: ResourceChangeDetail
properties_list:
- description: ''
  name: Target
  type: object
- description: ''
  name: Evaluation
  type: string
- description: ''
  name: ChangeSource
  type: string
- description: ''
  name: CausingEntity
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-resource-change-detail-schema.json
slug: cloudformation-resource-change-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourceChangeDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Target\": {\n      \"type\": \"object\"\n    },\n    \"Evaluation\": {\n      \"type\": \"string\"\n    },\n    \"ChangeSource\": {\n      \"type\": \"string\"\n    },\n    \"CausingEntity\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-resource-change-detail-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: ResourceChangeDetail
---
