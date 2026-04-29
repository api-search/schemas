---
description: Request to invite member accounts to a behavior graph
layout: schema
name: CreateMembersRequest
properties_list:
- description: The ARN of the behavior graph.
  name: GraphArn
  type: string
- description: Customized message text to include in the invitation email message.
  name: Message
  type: string
- description: If set to true, invitation emails are not sent.
  name: DisableEmailNotification
  type: boolean
- description: The list of AWS accounts to invite to become member accounts.
  name: Accounts
  type: array
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-create-members-request-schema.json
slug: amazon-detective-create-members-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-create-members-request-schema.json\",\n  \"title\": \"CreateMembersRequest\",\n  \"description\": \"Request to invite member accounts to a behavior graph\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"Message\": {\n      \"type\": \"string\",\n      \"description\": \"Customized message text to include in the invitation email message.\",\n      \"example\": \"Please join our security behavior graph.\"\n    },\n    \"DisableEmailNotification\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, invitation emails are not sent.\",\n      \"example\": false\n\
  \    },\n    \"Accounts\": {\n      \"type\": \"array\",\n      \"description\": \"The list of AWS accounts to invite to become member accounts.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Account\"\n      }\n    }\n  },\n  \"required\": [\n    \"GraphArn\",\n    \"Accounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-create-members-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: CreateMembersRequest
---
