---
description: Pagination cursor for next page
layout: schema
name: PagingNext
properties_list:
- description: Cursor token for the next page
  name: after
  type: string
- description: Link to the next page
  name: link
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-associations-paging-next-schema.json
slug: hubspot-crm-associations-paging-next
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Pagination cursor for next page\",\n  \"properties\": {\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor token for the next page\",\n      \"example\": \"example-value\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"description\": \"Link to the next page\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PagingNext\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-paging-next-schema.json
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
