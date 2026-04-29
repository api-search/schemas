---
description: ''
layout: schema
name: BodyWrite
properties_list:
- description: The representation format of the body content.
  name: representation
  type: string
- description: The body content in the specified representation.
  name: value
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-body-write-schema.json
slug: confluence-cloud-v2-body-write
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BodyWrite\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"representation\": {\n      \"type\": \"string\",\n      \"description\": \"The representation format of the body content.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The body content in the specified representation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-body-write-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: BodyWrite
---
