---
description: ''
layout: schema
name: PageUpdateRequest
properties_list:
- description: The ID of the page being updated.
  name: id
  type: string
- description: The status of the page.
  name: status
  type: string
- description: The new title of the page.
  name: title
  type: string
- description: The ID of the space the page belongs to.
  name: spaceId
  type: string
- description: The ID of the new parent page.
  name: parentId
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-page-update-request-schema.json
slug: confluence-cloud-v2-page-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the page being updated.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the page.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The new title of the page.\"\n    },\n    \"spaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the space the page belongs to.\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the new parent page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-page-update-request-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: PageUpdateRequest
---
