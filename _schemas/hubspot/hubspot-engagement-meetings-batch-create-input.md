---
description: ''
layout: schema
name: BatchCreateInput
properties_list:
- description: ''
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-meetings-batch-create-input-schema.json
slug: hubspot-engagement-meetings-batch-create-input
source_filename: hubspot-engagement-meetings-batch-create-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"properties\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"properties\": {\n            \"type\": \"object\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchCreateInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-meetings-batch-create-input-schema.json
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
