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
schema_file: json-schema/hubspot-marketing-emal-paging-schema.json
slug: hubspot-marketing-emal-paging
source_filename: hubspot-marketing-emal-paging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Pagination information\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the next page\",\n      \"properties\": {\n        \"after\": {\n          \"type\": \"string\",\n          \"description\": \"Cursor for the next page\",\n          \"example\": \"c210cC10b2tlbi1hYmMxMjM%3D\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"Link to the next page\",\n          \"example\": \"https://app.hubspot.com/contacts/12345\"\n        }\n      },\n      \"required\": [\n        \"after\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Paging\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-marketing-emal-paging-schema.json
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
