---
description: Metadata for a file or folder in the CMS Developer File System
layout: schema
name: AssetFileMetadata
properties_list:
- description: The full path of the file in the CMS Developer File System
  name: id
  type: string
- description: The name of the file or folder
  name: name
  type: string
- description: Whether this path represents a folder (true) or file (false)
  name: folder
  type: boolean
- description: List of child files and folders (only present for folders)
  name: children
  type: array
- description: Content hash for change detection
  name: hash
  type: string
- description: Unix timestamp when the file was created
  name: createdAt
  type: integer
- description: Unix timestamp when the file was last updated
  name: updatedAt
  type: integer
- description: Unix timestamp when the file was archived (if applicable)
  name: archivedAt
  type: integer
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-source-code-asset-file-metadata-schema.json
slug: hubspot-source-code-asset-file-metadata
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Metadata for a file or folder in the CMS Developer File System\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The full path of the file in the CMS Developer File System\",\n      \"example\": \"templates/blog/post.html\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file or folder\",\n      \"example\": \"post.html\"\n    },\n    \"folder\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this path represents a folder (true) or file (false)\",\n      \"example\": false\n    },\n    \"children\": {\n      \"type\": \"array\",\n      \"description\": \"List of child files and folders (only present for folders)\",\n      \"example\": [\n        \"header.html\",\n        \"footer.html\",\n        \"sidebar.html\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"hash\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Content hash for change detection\",\n      \"example\": \"a1b2c3d4e5f6\"\n    },\n    \"createdAt\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the file was created\",\n      \"format\": \"int64\",\n      \"example\": 1705312200000\n    },\n    \"updatedAt\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the file was last updated\",\n      \"format\": \"int64\",\n      \"example\": 1705398600000\n    },\n    \"archivedAt\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the file was archived (if applicable)\",\n      \"format\": \"int64\",\n      \"example\": 0\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"folder\",\n    \"createdAt\",\n    \"updatedAt\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssetFileMetadata\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-source-code-asset-file-metadata-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: AssetFileMetadata
---
