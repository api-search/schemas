---
description: Input for a batch read operation.
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
schema_file: json-schema/crm-deals-api-batch-read-input-schema.json
slug: crm-deals-api-batch-read-input
source_filename: crm-deals-api-batch-read-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-deals-api-batch-read-input-schema.json\",\n  \"title\": \"BatchReadInput\",\n  \"description\": \"Input for a batch read operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    },\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-deals-api-batch-read-input-schema.json
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
