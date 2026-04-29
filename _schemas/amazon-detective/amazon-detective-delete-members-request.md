---
description: Request to remove member accounts from a behavior graph
layout: schema
name: DeleteMembersRequest
properties_list:
- description: The ARN of the behavior graph to remove members from.
  name: GraphArn
  type: string
- description: The list of AWS account identifiers of the member accounts to remove.
  name: AccountIds
  type: array
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-delete-members-request-schema.json
slug: amazon-detective-delete-members-request
source_filename: amazon-detective-delete-members-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-delete-members-request-schema.json\",\n  \"title\": \"DeleteMembersRequest\",\n  \"description\": \"Request to remove member accounts from a behavior graph\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph to remove members from.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"AccountIds\": {\n      \"type\": \"array\",\n      \"description\": \"The list of AWS account identifiers of the member accounts to remove.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"234567890123\"\n      ]\n    }\n  },\n  \"required\": [\n    \"GraphArn\",\n    \"AccountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-delete-members-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: DeleteMembersRequest
---
