---
description: Pagination information
layout: schema
name: Paging
properties_list:
- description: ''
  name: next
  type: object
- description: ''
  name: prev
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-payments-paging-schema.json
slug: hubspot-commerce-payments-paging
source_filename: hubspot-commerce-payments-paging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Pagination information\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"after\": \"example-value\",\n        \"link\": \"https://app.hubspot.com/contacts/12345\"\n      },\n      \"properties\": {\n        \"after\": {\n          \"type\": \"string\",\n          \"description\": \"Cursor for the next page\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"Link to the next page\"\n        }\n      }\n    },\n    \"prev\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"before\": \"example-value\",\n        \"link\": \"https://app.hubspot.com/contacts/12345\"\n      },\n      \"properties\": {\n        \"before\": {\n          \"type\": \"string\",\n          \"description\": \"Cursor for the previous page\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"Link to the\
  \ previous page\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Paging\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-paging-schema.json
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
