---
description: ''
layout: schema
name: BatchReadInput
properties_list:
- description: ''
  name: properties
  type: array
- description: ''
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-meetings-batch-read-input-schema.json
slug: hubspot-engagement-meetings-batch-read-input
source_filename: hubspot-engagement-meetings-batch-read-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"array\",\n      \"example\": [\n        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"inputs\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"id\": \"500123\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchReadInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-meetings-batch-read-input-schema.json
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
title: BatchReadInput
---
