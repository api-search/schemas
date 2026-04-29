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
schema_file: json-schema/crm-deals-api-paging-schema.json
slug: crm-deals-api-paging
source_filename: crm-deals-api-paging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-deals-api-paging-schema.json\",\n  \"title\": \"Paging\",\n  \"description\": \"Pagination information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"after\": {\n          \"type\": \"string\"\n        }\n      },\n      \"example\": {\n        \"after\": \"example-value\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-deals-api-paging-schema.json
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
