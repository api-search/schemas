---
description: List of group members.
layout: schema
name: GroupMemberListResponse
properties_list:
- description: ''
  name: data
  type: array
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-group-member-list-response-schema.json
slug: bettercloud-group-member-list-response
source_filename: bettercloud-group-member-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-member-list-response-schema.json\",\n  \"title\": \"GroupMemberListResponse\",\n  \"description\": \"List of group members.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GroupMember\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-member-list-response-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: GroupMemberListResponse
---
