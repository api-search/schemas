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
schema_file: json-schema/hubspot-conversations-paging-next-schema.json
slug: hubspot-conversations-paging-next
source_filename: hubspot-conversations-paging-next-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Pagination cursor information for retrieving the next page.\",\n  \"properties\": {\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor token for the next page\",\n      \"example\": \"NTI1Cg%3D%3D\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"description\": \"API link to the next page\",\n      \"example\": \"/conversations/v3/conversations/inboxes?after=NTI1Cg%3D%3D\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PagingNext\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-conversations-paging-next-schema.json
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
