---
description: Individual item in a batch delete request
layout: schema
name: BatchDeleteInputItem
properties_list:
- description: The unique identifier for the HubSpot portal (account)
  name: portalId
  type: integer
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-feature-flags-batch-delete-input-item-schema.json
slug: hubspot-crm-feature-flags-batch-delete-input-item
source_filename: hubspot-crm-feature-flags-batch-delete-input-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Individual item in a batch delete request\",\n  \"properties\": {\n    \"portalId\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier for the HubSpot portal (account)\",\n      \"format\": \"int64\",\n      \"example\": 98765432\n    }\n  },\n  \"required\": [\n    \"portalId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchDeleteInputItem\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-batch-delete-input-item-schema.json
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
title: BatchDeleteInputItem
---
