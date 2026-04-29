---
description: Metadata object for page, blogpost, comment content
layout: schema
name: ContentMetadata
properties_list:
- description: ''
  name: currentuser
  type: object
- description: ''
  name: frontend
  type: object
- description: ''
  name: labels
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-metadata-schema.json
slug: atlassian-confluence-content-content-metadata
source_filename: atlassian-confluence-content-content-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentMetadata\",\n  \"type\": \"object\",\n  \"description\": \"Metadata object for page, blogpost, comment content\",\n  \"properties\": {\n    \"currentuser\": {\n      \"type\": \"object\"\n    },\n    \"frontend\": {\n      \"type\": \"object\"\n    },\n    \"labels\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-metadata-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentMetadata
---
