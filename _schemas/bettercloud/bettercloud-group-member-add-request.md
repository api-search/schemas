---
description: Request body for adding a member to a group.
layout: schema
name: GroupMemberAddRequest
properties_list:
- description: ID of the user to add to the group.
  name: user_id
  type: string
- description: Role to assign in the group.
  name: role
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-group-member-add-request-schema.json
slug: bettercloud-group-member-add-request
source_filename: bettercloud-group-member-add-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-member-add-request-schema.json\",\n  \"title\": \"GroupMemberAddRequest\",\n  \"description\": \"Request body for adding a member to a group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user to add to the group.\",\n      \"example\": \"user-a1b2c3d4\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Role to assign in the group.\",\n      \"enum\": [\n        \"owner\",\n        \"manager\",\n        \"member\"\n      ],\n      \"example\": \"member\"\n    }\n  },\n  \"required\": [\n    \"user_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-member-add-request-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: GroupMemberAddRequest
---
