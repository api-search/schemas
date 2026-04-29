---
description: An attachment on an issue.
layout: schema
name: Attachment
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: filename
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: size
  type: integer
- description: ''
  name: mimeType
  type: string
- description: The URL to download the attachment content.
  name: content
  type: string
- description: ''
  name: thumbnail
  type: string
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-attachment-schema.json
slug: jira-cloud-platform-rest-attachment
source_filename: jira-cloud-platform-rest-attachment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Attachment\",\n  \"type\": \"object\",\n  \"description\": \"An attachment on an issue.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"filename\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"string\"\n    },\n    \"size\": {\n      \"type\": \"integer\"\n    },\n    \"mimeType\": {\n      \"type\": \"string\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to download the attachment content.\"\n    },\n    \"thumbnail\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-attachment-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Attachment
---
