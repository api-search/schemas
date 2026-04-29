---
description: ''
layout: schema
name: VersionWrite
properties_list:
- description: The new version number. Must be incremented by 1.
  name: number
  type: integer
- description: An optional message associated with this version.
  name: message
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-version-write-schema.json
slug: confluence-cloud-v2-version-write
source_filename: confluence-cloud-v2-version-write-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VersionWrite\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"number\": {\n      \"type\": \"integer\",\n      \"description\": \"The new version number. Must be incremented by 1.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"An optional message associated with this version.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-version-write-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: VersionWrite
---
