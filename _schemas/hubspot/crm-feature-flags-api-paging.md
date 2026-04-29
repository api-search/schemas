---
description: Pagination information for list responses
layout: schema
name: Paging
properties_list:
- description: Information for fetching the next page of results
  name: next
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-feature-flags-api-paging-schema.json
slug: crm-feature-flags-api-paging
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-paging-schema.json\",\n  \"title\": \"Paging\",\n  \"description\": \"Pagination information for list responses\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"object\",\n      \"description\": \"Information for fetching the next page of results\",\n      \"required\": [\n        \"after\"\n      ],\n      \"properties\": {\n        \"after\": {\n          \"type\": \"string\",\n          \"description\": \"Cursor for the next page\",\n          \"example\": \"NTI1Cg%3D%3D\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"Direct link to the next page\",\n          \"example\": \"https://api.hubapi.com/feature-flags/v3/12345678/flags/new-dashboard-feature/portals?after=NTI1Cg%3D%3D\"\n        }\n      }\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-paging-schema.json
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
