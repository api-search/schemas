---
description: Base schema for a Sanity Content Lake document. All documents in Content Lake include system-managed underscore-prefixed fields.
layout: schema
name: Sanity Document
properties_list:
- description: Unique document identifier. Drafts are prefixed with 'drafts.'
  name: _id
  type: string
- description: Document type identifier matching the schema definition
  name: _type
  type: string
- description: Revision identifier, updated on each mutation
  name: _rev
  type: string
- description: ISO 8601 timestamp of document creation
  name: _createdAt
  type: string
- description: ISO 8601 timestamp of last document update
  name: _updatedAt
  type: string
provider_name: Sanity
provider_slug: sanity
schema_file: json-schema/sanity-document-schema.json
slug: sanity-document
source_filename: sanity-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sanity/json-schema/document.json\",\n  \"title\": \"Sanity Document\",\n  \"description\": \"Base schema for a Sanity Content Lake document. All documents in Content Lake include system-managed underscore-prefixed fields.\",\n  \"type\": \"object\",\n  \"required\": [\"_id\", \"_type\"],\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique document identifier. Drafts are prefixed with 'drafts.'\",\n      \"examples\": [\"abc123\", \"drafts.abc123\"]\n    },\n    \"_type\": {\n      \"type\": \"string\",\n      \"description\": \"Document type identifier matching the schema definition\",\n      \"examples\": [\"post\", \"author\", \"page\", \"sanity.imageAsset\"]\n    },\n    \"_rev\": {\n      \"type\": \"string\",\n      \"description\": \"Revision identifier, updated on each mutation\"\n    },\n    \"_createdAt\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of document creation\"\n    },\n    \"_updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of last document update\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/json-schema/sanity-document-schema.json
tags:
- Headless CMS
- Content Management
- GROQ
- Real-Time
- Structured Content
- Developer Platform
title: Sanity Document
---
