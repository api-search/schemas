---
description: Request body for creating a group.
layout: schema
name: GroupCreateRequest
properties_list:
- description: Display name of the group.
  name: name
  type: string
- description: Email address of the group.
  name: email
  type: string
- description: Group description.
  name: description
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-group-create-request-schema.json
slug: bettercloud-group-create-request
source_filename: bettercloud-group-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-create-request-schema.json\",\n  \"title\": \"GroupCreateRequest\",\n  \"description\": \"Request body for creating a group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the group.\",\n      \"example\": \"New Team\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the group.\",\n      \"example\": \"newteam@example.com\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Group description.\",\n      \"example\": \"New team group\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-group-create-request-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: GroupCreateRequest
---
