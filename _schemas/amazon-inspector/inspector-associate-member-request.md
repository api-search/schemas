---
description: AssociateMemberRequest schema
layout: schema
name: AssociateMemberRequest
properties_list:
- description: ''
  name: accountId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-associate-member-request-schema.json
slug: inspector-associate-member-request
source_filename: inspector-associate-member-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-associate-member-request-schema.json\",\n  \"title\": \"AssociateMemberRequest\",\n  \"description\": \"AssociateMemberRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the member account to be associated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-associate-member-request-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AssociateMemberRequest
---
