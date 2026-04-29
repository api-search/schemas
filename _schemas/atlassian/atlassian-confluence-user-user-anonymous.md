---
description: ''
layout: schema
name: UserAnonymous
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: operations
  type: array
- description: Whether the user is an external collaborator user
  name: isExternalCollaborator
  type: boolean
- description: ''
  name: _expandable
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-user-user-anonymous-schema.json
slug: atlassian-confluence-user-user-anonymous
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserAnonymous\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"operations\": {\n      \"type\": \"array\"\n    },\n    \"isExternalCollaborator\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is an external collaborator user\"\n    },\n    \"_expandable\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-user-user-anonymous-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: UserAnonymous
---
