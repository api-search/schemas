---
description: Represents a group within an organization.
layout: schema
name: Group
properties_list:
- description: The unique identifier of the group.
  name: id
  type: string
- description: The resource type.
  name: type
  type: string
- description: The attributes of the group.
  name: attributes
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-group-schema.json
slug: atlassian-admin-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Group\",\n  \"type\": \"object\",\n  \"description\": \"Represents a group within an organization.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the group.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"The attributes of the group.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-group-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: Group
---
