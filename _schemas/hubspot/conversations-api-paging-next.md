---
description: Pagination cursor information for retrieving the next page.
layout: schema
name: PagingNext
properties_list:
- description: Cursor token for the next page
  name: after
  type: string
- description: API link to the next page
  name: link
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/conversations-api-paging-next-schema.json
slug: conversations-api-paging-next
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-paging-next-schema.json\",\n  \"title\": \"PagingNext\",\n  \"description\": \"Pagination cursor information for retrieving the next page.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor token for the next page\",\n      \"example\": \"NTI1Cg%3D%3D\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"description\": \"API link to the next page\",\n      \"example\": \"/conversations/v3/conversations/inboxes?after=NTI1Cg%3D%3D\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-paging-next-schema.json
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
title: PagingNext
---
