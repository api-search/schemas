---
description: ''
layout: schema
name: VersionRestore
properties_list:
- description: Set to 'restore'.
  name: operationKey
  type: string
- description: ''
  name: params
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-version-restore-schema.json
slug: atlassian-confluence-content-version-restore
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VersionRestore\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operationKey\": {\n      \"type\": \"string\",\n      \"description\": \"Set to 'restore'.\"\n    },\n    \"params\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-version-restore-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: VersionRestore
---
