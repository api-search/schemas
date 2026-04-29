---
description: The user or group that the permission applies to.
layout: schema
name: PermissionSubjectWithGroupId
properties_list:
- description: ''
  name: type
  type: string
- description: for `type=user`, identifier should be user's accountId or `anonymous` for anonymous users for `type=group`, identifier should be ID of the group
  name: identifier
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-permission-subject-with-group-id-schema.json
slug: atlassian-confluence-content-permission-subject-with-group-id
source_filename: atlassian-confluence-content-permission-subject-with-group-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PermissionSubjectWithGroupId\",\n  \"type\": \"object\",\n  \"description\": \"The user or group that the permission applies to.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"for `type=user`, identifier should be user's accountId or `anonymous` for anonymous users\\n\\nfor `type=group`, identifier should be ID of the group\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-permission-subject-with-group-id-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: PermissionSubjectWithGroupId
---
