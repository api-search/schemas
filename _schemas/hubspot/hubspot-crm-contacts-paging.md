---
description: Pagination information.
layout: schema
name: Paging
properties_list:
- description: ''
  name: next
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-contacts-paging-schema.json
slug: hubspot-crm-contacts-paging
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Pagination information.\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"after\": \"example-value\"\n      },\n      \"properties\": {\n        \"after\": {\n          \"type\": \"string\",\n          \"description\": \"The cursor to use to get the next page of results.\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Paging\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-contacts-paging-schema.json
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
