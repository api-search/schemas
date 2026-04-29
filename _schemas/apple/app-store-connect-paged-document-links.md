---
description: ''
layout: schema
name: PagedDocumentLinks
properties_list:
- description: The URL for the current page of results
  name: self
  type: string
- description: The URL for the first page of results
  name: first
  type: string
- description: The URL for the next page of results
  name: next
  type: string
provider_name: Apple
provider_slug: apple
schema_file: json-schema/app-store-connect-paged-document-links-schema.json
slug: app-store-connect-paged-document-links
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PagedDocumentLinks\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\",\n      \"description\": \"The URL for the current page of results\"\n    },\n    \"first\": {\n      \"type\": \"string\",\n      \"description\": \"The URL for the first page of results\"\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"description\": \"The URL for the next page of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple/refs/heads/main/json-schema/app-store-connect-paged-document-links-schema.json
tags:
- Developer
- iOS
- macOS
- Mobile
- Technology
title: PagedDocumentLinks
---
