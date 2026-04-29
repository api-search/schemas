---
description: SearchDocument schema from Backstage search API
layout: schema
name: SearchDocument
properties_list:
- description: Title of the document.
  name: title
  type: string
- description: Text content of the document.
  name: text
  type: string
- description: URL or path to the original content.
  name: location
  type: string
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/search-search-document-schema.json
slug: search-search-document
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/search-search-document-schema.json\",\n  \"title\": \"SearchDocument\",\n  \"description\": \"SearchDocument schema from Backstage search API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the document.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Text content of the document.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"URL or path to the original content.\"\n    }\n  },\n  \"required\": [\n    \"title\",\n    \"text\",\n    \"location\"\n  ],\n  \"additionalProperties\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/search-search-document-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: SearchDocument
---
