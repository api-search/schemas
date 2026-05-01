---
description: DisassociateMemberResponse schema
layout: schema
name: DisassociateMemberResponse
properties_list:
- description: ''
  name: accountId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-disassociate-member-response-schema.json
slug: inspector-disassociate-member-response
source_filename: inspector-disassociate-member-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-disassociate-member-response-schema.json\",\n  \"title\": \"DisassociateMemberResponse\",\n  \"description\": \"DisassociateMemberResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the successfully disassociated member.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-disassociate-member-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: DisassociateMemberResponse
---
