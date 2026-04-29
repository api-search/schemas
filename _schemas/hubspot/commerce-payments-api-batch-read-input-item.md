---
description: A single input item for batch read
layout: schema
name: BatchReadInputItem
properties_list:
- description: The ID of the payment to read
  name: id
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/commerce-payments-api-batch-read-input-item-schema.json
slug: commerce-payments-api-batch-read-input-item
source_filename: commerce-payments-api-batch-read-input-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-batch-read-input-item-schema.json\",\n  \"title\": \"BatchReadInputItem\",\n  \"description\": \"A single input item for batch read\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the payment to read\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-batch-read-input-item-schema.json
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
title: BatchReadInputItem
---
