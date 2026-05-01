---
description: GetMemberResponse schema
layout: schema
name: GetMemberResponse
properties_list:
- description: ''
  name: member
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-get-member-response-schema.json
slug: inspector-get-member-response
source_filename: inspector-get-member-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-get-member-response-schema.json\",\n  \"title\": \"GetMemberResponse\",\n  \"description\": \"GetMemberResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"member\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Member\"\n        },\n        {\n          \"description\": \"Details of the retrieved member account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-get-member-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: GetMemberResponse
---
