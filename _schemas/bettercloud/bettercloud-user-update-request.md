---
description: Fields to update on a user (all optional).
layout: schema
name: UserUpdateRequest
properties_list:
- description: New first name.
  name: first_name
  type: string
- description: New last name.
  name: last_name
  type: string
- description: New department.
  name: department
  type: string
- description: New job title.
  name: title
  type: string
- description: New office location.
  name: location
  type: string
provider_name: BetterCloud
provider_slug: bettercloud
schema_file: json-schema/bettercloud-user-update-request-schema.json
slug: bettercloud-user-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-user-update-request-schema.json\",\n  \"title\": \"UserUpdateRequest\",\n  \"description\": \"Fields to update on a user (all optional).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"New first name.\",\n      \"example\": \"Jane\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"New last name.\",\n      \"example\": \"Smith\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"New department.\",\n      \"example\": \"Product\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"New job title.\",\n      \"example\": \"Product Manager\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"\
  New office location.\",\n      \"example\": \"New York\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/json-schema/bettercloud-user-update-request-schema.json
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
title: UserUpdateRequest
---
