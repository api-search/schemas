---
description: Pagination links for cursor-based pagination.
layout: schema
name: PaginationLinks
properties_list:
- description: URL for the next page of results. Contains the cursor parameter.
  name: next
  type: string
- description: The base URL of the Confluence instance.
  name: base
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-pagination-links-schema.json
slug: confluence-cloud-v2-pagination-links
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginationLinks\",\n  \"type\": \"object\",\n  \"description\": \"Pagination links for cursor-based pagination.\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"string\",\n      \"description\": \"URL for the next page of results. Contains the cursor parameter.\"\n    },\n    \"base\": {\n      \"type\": \"string\",\n      \"description\": \"The base URL of the Confluence instance.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-pagination-links-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: PaginationLinks
---
