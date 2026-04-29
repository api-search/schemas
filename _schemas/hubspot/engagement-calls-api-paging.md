---
description: Pagination information
layout: schema
name: Paging
properties_list:
- description: Information about the next page
  name: next
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-calls-api-paging-schema.json
slug: engagement-calls-api-paging
source_filename: engagement-calls-api-paging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-paging-schema.json\",\n  \"title\": \"Paging\",\n  \"description\": \"Pagination information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the next page\",\n      \"required\": [\n        \"after\"\n      ],\n      \"properties\": {\n        \"after\": {\n          \"type\": \"string\",\n          \"description\": \"Cursor for the next page\",\n          \"example\": \"NTI1Cg%3D%3D\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"Link to the next page\",\n          \"example\": \"https://app.hubspot.com/contacts/12345\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-paging-schema.json
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
