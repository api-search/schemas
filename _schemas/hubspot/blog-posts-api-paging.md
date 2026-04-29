---
description: Pagination information
layout: schema
name: Paging
properties_list:
- description: Pagination cursor for next page
  name: next
  type: object
- description: Pagination cursor for previous page
  name: prev
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/blog-posts-api-paging-schema.json
slug: blog-posts-api-paging
source_filename: blog-posts-api-paging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-paging-schema.json\",\n  \"title\": \"Paging\",\n  \"description\": \"Pagination information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination cursor for next page\",\n      \"properties\": {\n        \"after\": {\n          \"type\": \"string\",\n          \"description\": \"Cursor token for the next page\",\n          \"example\": \"example-value\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"API link to the next page\",\n          \"example\": \"https://app.hubspot.com/contacts/12345\"\n        }\n      }\n    },\n    \"prev\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination cursor for previous page\",\n      \"properties\": {\n        \"before\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Cursor token for the previous page\",\n          \"example\": \"example-value\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"API link to the previous page\",\n          \"example\": \"https://app.hubspot.com/contacts/12345\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-paging-schema.json
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
title: Paging
---
