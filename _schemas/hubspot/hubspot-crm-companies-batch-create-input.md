---
description: Input for a batch create operation.
layout: schema
name: BatchCreateInput
properties_list:
- description: ''
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-companies-batch-create-input-schema.json
slug: hubspot-crm-companies-batch-create-input
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input for a batch create operation.\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"properties\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Input for creating or updating a CRM object.\",\n        \"properties\": {\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The properties to set on the object.\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchCreateInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-companies-batch-create-input-schema.json
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
title: BatchCreateInput
---
