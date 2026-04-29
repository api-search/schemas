---
description: ''
layout: schema
name: StackInstanceSummary
properties_list:
- description: ''
  name: StackSetId
  type: string
- description: ''
  name: Region
  type: string
- description: ''
  name: Account
  type: string
- description: ''
  name: StackId
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: StatusReason
  type: string
- description: ''
  name: DriftStatus
  type: string
- description: ''
  name: LastDriftCheckTimestamp
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-instance-summary-schema.json
slug: cloudformation-stack-instance-summary
source_filename: cloudformation-stack-instance-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackInstanceSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackSetId\": {\n      \"type\": \"string\"\n    },\n    \"Region\": {\n      \"type\": \"string\"\n    },\n    \"Account\": {\n      \"type\": \"string\"\n    },\n    \"StackId\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\"\n    },\n    \"StatusReason\": {\n      \"type\": \"string\"\n    },\n    \"DriftStatus\": {\n      \"type\": \"string\"\n    },\n    \"LastDriftCheckTimestamp\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-instance-summary-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: StackInstanceSummary
---
