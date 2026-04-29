---
description: Represents a role assignment for a user.
layout: schema
name: RoleAssignment
properties_list:
- description: The role identifier.
  name: role
  type: string
- description: The resource the role is assigned to.
  name: resource
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-role-assignment-schema.json
slug: atlassian-admin-role-assignment
source_filename: atlassian-admin-role-assignment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RoleAssignment\",\n  \"type\": \"object\",\n  \"description\": \"Represents a role assignment for a user.\",\n  \"properties\": {\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The role identifier.\"\n    },\n    \"resource\": {\n      \"type\": \"object\",\n      \"description\": \"The resource the role is assigned to.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-role-assignment-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: RoleAssignment
---
