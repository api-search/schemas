---
description: Input for reading a single item in a batch
layout: schema
name: BatchReadInput
properties_list:
- description: The call identifier
  name: id
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-calls-api-batch-read-input-schema.json
slug: engagement-calls-api-batch-read-input
source_filename: engagement-calls-api-batch-read-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-batch-read-input-schema.json\",\n  \"title\": \"BatchReadInput\",\n  \"description\": \"Input for reading a single item in a batch\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The call identifier\",\n      \"example\": \"512\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-batch-read-input-schema.json
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
