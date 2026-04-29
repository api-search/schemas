---
description: Version information for content.
layout: schema
name: Version
properties_list:
- description: The ISO 8601 timestamp of this version.
  name: createdAt
  type: string
- description: The message associated with this version.
  name: message
  type: string
- description: The version number.
  name: number
  type: integer
- description: Whether this was a minor edit.
  name: minorEdit
  type: boolean
- description: The Atlassian account ID of the version author.
  name: authorId
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-version-schema.json
slug: confluence-cloud-v2-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Version\",\n  \"type\": \"object\",\n  \"description\": \"Version information for content.\",\n  \"properties\": {\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 8601 timestamp of this version.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The message associated with this version.\"\n    },\n    \"number\": {\n      \"type\": \"integer\",\n      \"description\": \"The version number.\"\n    },\n    \"minorEdit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this was a minor edit.\"\n    },\n    \"authorId\": {\n      \"type\": \"string\",\n      \"description\": \"The Atlassian account ID of the version author.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-version-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: Version
---
