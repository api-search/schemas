---
description: Represents a comment in a Word document.
layout: schema
name: Comment
properties_list:
- description: Unique identifier of the comment.
  name: id
  type: string
- description: Name of the comment author.
  name: authorName
  type: string
- description: Email of the comment author.
  name: authorEmail
  type: string
- description: Text content of the comment.
  name: content
  type: string
- description: When the comment was created.
  name: createdDate
  type: string
- description: Whether the comment has been resolved.
  name: resolved
  type: boolean
provider_name: Microsoft Word
provider_slug: microsoft-word
schema_file: json-schema/javascript-api-comment-schema.json
slug: javascript-api-comment
source_filename: javascript-api-comment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/javascript-api-comment-schema.json\",\n  \"title\": \"Comment\",\n  \"description\": \"Represents a comment in a Word document.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the comment.\"\n    },\n    \"authorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the comment author.\"\n    },\n    \"authorEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email of the comment author.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Text content of the comment.\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the comment was created.\"\n\
  \    },\n    \"resolved\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the comment has been resolved.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/javascript-api-comment-schema.json
tags:
- Documents
- Microsoft 365
- Office
- Productivity
- Word Processing
title: Comment
---
