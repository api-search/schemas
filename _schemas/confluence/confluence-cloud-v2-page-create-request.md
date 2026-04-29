---
description: ''
layout: schema
name: PageCreateRequest
properties_list:
- description: The ID of the space to create the page in.
  name: spaceId
  type: string
- description: The status of the page.
  name: status
  type: string
- description: The title of the page.
  name: title
  type: string
- description: The ID of the parent page. If omitted, the page will be a root-level page.
  name: parentId
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-page-create-request-schema.json
slug: confluence-cloud-v2-page-create-request
source_filename: confluence-cloud-v2-page-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the space to create the page in.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the page.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the page.\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the parent page. If omitted, the page will be a root-level page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-page-create-request-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: PageCreateRequest
---
