---
description: AssociateMemberResponse schema
layout: schema
name: AssociateMemberResponse
properties_list:
- description: ''
  name: accountId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-associate-member-response-schema.json
slug: inspector-associate-member-response
source_filename: inspector-associate-member-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-associate-member-response-schema.json\",\n  \"title\": \"AssociateMemberResponse\",\n  \"description\": \"AssociateMemberResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the successfully associated member account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-associate-member-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AssociateMemberResponse
---
