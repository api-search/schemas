---
description: Shows whether a piece of content has attachments, comments, or child pages/whiteboards. Note, this doesn't actually contain the child objects.
layout: schema
name: ContentChildType
properties_list:
- description: ''
  name: attachment
  type: object
- description: ''
  name: comment
  type: object
- description: ''
  name: page
  type: object
- description: ''
  name: _expandable
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-child-type-schema.json
slug: atlassian-confluence-content-content-child-type
source_filename: atlassian-confluence-content-content-child-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentChildType\",\n  \"type\": \"object\",\n  \"description\": \"Shows whether a piece of content has attachments, comments, or child pages/whiteboards.\\nNote, this doesn't actually contain the child objects.\",\n  \"properties\": {\n    \"attachment\": {\n      \"type\": \"object\"\n    },\n    \"comment\": {\n      \"type\": \"object\"\n    },\n    \"page\": {\n      \"type\": \"object\"\n    },\n    \"_expandable\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-child-type-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentChildType
---
