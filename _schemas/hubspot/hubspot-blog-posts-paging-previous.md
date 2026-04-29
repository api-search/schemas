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
schema_file: json-schema/hubspot-blog-posts-paging-previous-schema.json
slug: hubspot-blog-posts-paging-previous
source_filename: hubspot-blog-posts-paging-previous-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Pagination cursor for previous page\",\n  \"properties\": {\n    \"before\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor token for the previous page\",\n      \"example\": \"example-value\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"description\": \"API link to the previous page\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PagingPrevious\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-blog-posts-paging-previous-schema.json
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
