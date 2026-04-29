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
schema_file: json-schema/hubspot-commerce-payments-batch-read-input-item-schema.json
slug: hubspot-commerce-payments-batch-read-input-item
source_filename: hubspot-commerce-payments-batch-read-input-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A single input item for batch read\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the payment to read\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchReadInputItem\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-batch-read-input-item-schema.json
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
