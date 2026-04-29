---
description: This essentially the same as the `User` object, but no `_links` property and no `_expandable` property (therefore, different required fields).
layout: schema
name: WatchUser
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: timeZone
  type: string
- description: ''
  name: operations
  type: array
- description: ''
  name: isExternalCollaborator
  type: boolean
- description: ''
  name: accountType
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: publicName
  type: string
- description: ''
  name: personalSpace
  type: object
- description: ''
  name: externalCollaborator
  type: boolean
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-watch-user-schema.json
slug: atlassian-confluence-content-watch-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WatchUser\",\n  \"type\": \"object\",\n  \"description\": \"This essentially the same as the `User` object, but no `_links` property and\\nno `_expandable` property (therefore, different required fields).\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\"\n    },\n    \"operations\": {\n      \"type\": \"array\"\n    },\n    \"isExternalCollaborator\": {\n      \"type\": \"boolean\"\n    },\n    \"accountType\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"publicName\": {\n      \"type\": \"string\"\n    },\n    \"personalSpace\": {\n      \"type\": \"object\"\n    },\n    \"externalCollaborator\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-watch-user-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: WatchUser
---
