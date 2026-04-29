---
description: This object represents an icon. If used as a profilePicture, this may be returned as null, depending on the user's privacy setting.
layout: schema
name: Icon
properties_list:
- description: ''
  name: path
  type: string
- description: ''
  name: width
  type: integer
- description: ''
  name: height
  type: integer
- description: ''
  name: isDefault
  type: boolean
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-icon-schema.json
slug: atlassian-confluence-content-icon
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Icon\",\n  \"type\": \"object\",\n  \"description\": \"This object represents an icon. If used as a profilePicture, this may be returned as null, depending on the user's privacy setting.\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"width\": {\n      \"type\": \"integer\"\n    },\n    \"height\": {\n      \"type\": \"integer\"\n    },\n    \"isDefault\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-icon-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: Icon
---
