---
description: Pagination information for the response.
layout: schema
name: Paging
properties_list:
- description: Information for retrieving the next page of results.
  name: next
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-search-paging-schema.json
slug: hubspot-crm-search-paging
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Pagination information for the response.\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"object\",\n      \"description\": \"Information for retrieving the next page of results.\",\n      \"example\": {\n        \"after\": \"example-value\",\n        \"link\": \"https://app.hubspot.com/contacts/12345\"\n      },\n      \"properties\": {\n        \"after\": {\n          \"type\": \"string\",\n          \"description\": \"The cursor token to use in the after parameter for the next page.\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"A URL link to the next page of results.\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Paging\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-search-paging-schema.json
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
