---
description: An organization admin account for Amazon Detective
layout: schema
name: Administrator
properties_list:
- description: The AWS account identifier of the Detective administrator account.
  name: AccountId
  type: string
- description: The ARN of the organization behavior graph.
  name: GraphArn
  type: string
- description: The date and time when the Detective administrator account was enabled.
  name: DelegationTime
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-administrator-schema.json
slug: amazon-detective-administrator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-administrator-schema.json\",\n  \"title\": \"Administrator\",\n  \"description\": \"An organization admin account for Amazon Detective\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account identifier of the Detective administrator account.\",\n      \"example\": \"123456789012\"\n    },\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the organization behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"DelegationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the Detective administrator account was enabled.\",\n      \"example\"\
  : \"2025-01-15T10:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-administrator-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: Administrator
---
