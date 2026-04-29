---
description: Pagination information for list responses.
layout: schema
name: Paging
properties_list:
- description: Pagination cursor information for retrieving the next page.
  name: next
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/conversations-api-paging-schema.json
slug: conversations-api-paging
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-paging-schema.json\",\n  \"title\": \"Paging\",\n  \"description\": \"Pagination information for list responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination cursor information for retrieving the next page.\",\n      \"properties\": {\n        \"after\": {\n          \"type\": \"string\",\n          \"description\": \"Cursor token for the next page\",\n          \"example\": \"NTI1Cg%3D%3D\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"API link to the next page\",\n          \"example\": \"/conversations/v3/conversations/inboxes?after=NTI1Cg%3D%3D\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/conversations-api-paging-schema.json
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
