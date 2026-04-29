---
description: ''
layout: schema
name: AttachmentPropertiesUpdateBody
properties_list:
- description: ''
  name: id
  type: string
- description: Set this to "attachment"
  name: type
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: extensions
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-attachment-properties-update-body-schema.json
slug: atlassian-confluence-content-attachment-properties-update-body
source_filename: atlassian-confluence-content-attachment-properties-update-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AttachmentPropertiesUpdateBody\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Set this to \\\"attachment\\\"\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\"\n    },\n    \"extensions\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-attachment-properties-update-body-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: AttachmentPropertiesUpdateBody
---
