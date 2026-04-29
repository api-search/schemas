---
description: Pagination cursor for previous page
layout: schema
name: PagingPrevious
properties_list:
- description: Cursor token for the previous page
  name: before
  type: string
- description: API link to the previous page
  name: link
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/blog-posts-api-paging-previous-schema.json
slug: blog-posts-api-paging-previous
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-paging-previous-schema.json\",\n  \"title\": \"PagingPrevious\",\n  \"description\": \"Pagination cursor for previous page\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"before\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor token for the previous page\",\n      \"example\": \"example-value\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"description\": \"API link to the previous page\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-paging-previous-schema.json
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
title: PagingPrevious
---
