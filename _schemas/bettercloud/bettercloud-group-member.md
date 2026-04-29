---
description: A member of a group.
layout: schema
name: GroupMember
properties_list:
- description: Unique identifier of the user.
  name: user_id
  type: string
- description: Email of the group member.
  name: email
  type: string
- description: Display name of the member.
  name: name
  type: string
- description: Role in the group.
  name: role
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-group-member-schema.json
slug: bettercloud-group-member
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-member-schema.json\",\n  \"title\": \"GroupMember\",\n  \"description\": \"A member of a group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the user.\",\n      \"example\": \"user-a1b2c3d4\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email of the group member.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the member.\",\n      \"example\": \"Jane Smith\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Role in the group.\",\n      \"enum\": [\n        \"owner\",\n        \"manager\",\n        \"member\"\
  \n      ],\n      \"example\": \"member\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-member-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: GroupMember
---
