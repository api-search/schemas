---
description: Represents a file attachment on Confluence content.
layout: schema
name: Attachment
properties_list:
- description: The unique identifier of the attachment.
  name: id
  type: string
- description: The status of the attachment.
  name: status
  type: string
- description: The filename of the attachment.
  name: title
  type: string
- description: The MIME type of the attachment.
  name: mediaType
  type: string
- description: Human-readable description of the media type.
  name: mediaTypeDescription
  type: string
- description: Comment associated with the attachment upload.
  name: comment
  type: string
- description: File size in bytes.
  name: fileSize
  type: integer
- description: The web UI link for viewing the attachment.
  name: webuiLink
  type: string
- description: The download link for the attachment.
  name: downloadLink
  type: string
- description: The ID of the page this attachment belongs to.
  name: pageId
  type: string
- description: The ID of the blog post this attachment belongs to.
  name: blogPostId
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-attachment-schema.json
slug: confluence-cloud-v2-attachment
source_filename: confluence-cloud-v2-attachment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Attachment\",\n  \"type\": \"object\",\n  \"description\": \"Represents a file attachment on Confluence content.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the attachment.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the attachment.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The filename of the attachment.\"\n    },\n    \"mediaType\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the attachment.\"\n    },\n    \"mediaTypeDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the media type.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comment associated with the attachment upload.\"\n    },\n    \"fileSize\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"File size in bytes.\"\n    },\n    \"webuiLink\": {\n      \"type\": \"string\",\n      \"description\": \"The web UI link for viewing the attachment.\"\n    },\n    \"downloadLink\": {\n      \"type\": \"string\",\n      \"description\": \"The download link for the attachment.\"\n    },\n    \"pageId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the page this attachment belongs to.\"\n    },\n    \"blogPostId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the blog post this attachment belongs to.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-attachment-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: Attachment
---
