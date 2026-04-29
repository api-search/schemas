---
description: Input for a batch archive operation.
layout: schema
name: BatchArchiveInput
properties_list:
- description: ''
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-companies-api-batch-archive-input-schema.json
slug: crm-companies-api-batch-archive-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-companies-api-batch-archive-input-schema.json\",\n  \"title\": \"BatchArchiveInput\",\n  \"description\": \"Input for a batch archive operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-companies-api-batch-archive-input-schema.json
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
title: BatchArchiveInput
---
