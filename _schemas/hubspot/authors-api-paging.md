---
description: Pagination information for navigating result sets
layout: schema
name: Paging
properties_list:
- description: Pagination cursor for retrieving the next page of results
  name: next
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/authors-api-paging-schema.json
slug: authors-api-paging
source_filename: authors-api-paging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-paging-schema.json\",\n  \"title\": \"Paging\",\n  \"description\": \"Pagination information for navigating result sets\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination cursor for retrieving the next page of results\",\n      \"properties\": {\n        \"after\": {\n          \"type\": \"string\",\n          \"description\": \"Cursor token for the next page\",\n          \"example\": \"example-value\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"API link to the next page of results\",\n          \"example\": \"https://app.hubspot.com/contacts/12345\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-paging-schema.json
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
