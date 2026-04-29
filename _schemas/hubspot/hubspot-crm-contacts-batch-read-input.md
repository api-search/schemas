---
description: Input for a batch read operation.
layout: schema
name: BatchReadInput
properties_list:
- description: The properties to return for each record.
  name: properties
  type: array
- description: The IDs of the records to read.
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-contacts-batch-read-input-schema.json
slug: hubspot-crm-contacts-batch-read-input
source_filename: hubspot-crm-contacts-batch-read-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input for a batch read operation.\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"The properties to return for each record.\",\n      \"example\": [\n        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of the records to read.\",\n      \"example\": [\n        {\n          \"id\": \"500123\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchReadInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-contacts-batch-read-input-schema.json
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
