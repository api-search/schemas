---
description: Input for reading a single item in a batch
layout: schema
name: BatchReadInput
properties_list:
- description: The note identifier
  name: id
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-notes-batch-read-input-schema.json
slug: hubspot-engagement-notes-batch-read-input
source_filename: hubspot-engagement-notes-batch-read-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input for reading a single item in a batch\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The note identifier\",\n      \"example\": \"1024\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchReadInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-notes-batch-read-input-schema.json
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
