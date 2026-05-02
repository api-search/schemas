---
description: A single documentation search result returned by the search_docs tool, containing a matching document's URL and relevant content.
layout: schema
name: grounded.tools Search Result
properties_list:
- description: URL of the matching document.
  name: url
  type: string
- description: Matching content from the document in Markdown format.
  name: content
  type: string
provider_name: Grounded.tools
provider_slug: grounded-tools
schema_file: json-schema/search-result.json
slug: search-result
source_filename: search-result.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/grounded-tools/blob/main/json-schema/search-result.json\",\n  \"title\": \"grounded.tools Search Result\",\n  \"description\": \"A single documentation search result returned by the search_docs tool, containing a matching document's URL and relevant content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the matching document.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Matching content from the document in Markdown format.\"\n    }\n  },\n  \"required\": [\n    \"url\",\n    \"content\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/grounded-tools/refs/heads/main/json-schema/search-result.json
tags:
- Developer Tools
- Developers
- Documentation
- Experience
title: grounded.tools Search Result
---
