---
description: ListMembersResponse schema
layout: schema
name: ListMembersResponse
properties_list:
- description: ''
  name: members
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-list-members-response-schema.json
slug: inspector-list-members-response
source_filename: inspector-list-members-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-members-response-schema.json\",\n  \"title\": \"ListMembersResponse\",\n  \"description\": \"ListMembersResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"members\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberList\"\n        },\n        {\n          \"description\": \"An object that contains details for each member account.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination parameter to be used on the next list operation to retrieve more items.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-members-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ListMembersResponse
---
