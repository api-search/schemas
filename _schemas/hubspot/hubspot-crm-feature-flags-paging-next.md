---
description: Information for fetching the next page of results
layout: schema
name: PagingNext
properties_list:
- description: Cursor for the next page
  name: after
  type: string
- description: Direct link to the next page
  name: link
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-feature-flags-paging-next-schema.json
slug: hubspot-crm-feature-flags-paging-next
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Information for fetching the next page of results\",\n  \"properties\": {\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page\",\n      \"example\": \"NTI1Cg%3D%3D\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"description\": \"Direct link to the next page\",\n      \"example\": \"https://api.hubapi.com/feature-flags/v3/12345678/flags/new-dashboard-feature/portals?after=NTI1Cg%3D%3D\"\n    }\n  },\n  \"required\": [\n    \"after\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PagingNext\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-paging-next-schema.json
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
