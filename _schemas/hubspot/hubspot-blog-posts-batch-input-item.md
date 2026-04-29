---
description: Single item in a batch archive operation
layout: schema
name: BatchInputItem
properties_list:
- description: ID of the post to process
  name: id
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-blog-posts-batch-input-item-schema.json
slug: hubspot-blog-posts-batch-input-item
source_filename: hubspot-blog-posts-batch-input-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Single item in a batch archive operation\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the post to process\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchInputItem\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-blog-posts-batch-input-item-schema.json
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
title: BatchInputItem
---
