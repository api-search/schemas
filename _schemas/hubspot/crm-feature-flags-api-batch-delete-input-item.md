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
schema_file: json-schema/crm-feature-flags-api-batch-delete-input-item-schema.json
slug: crm-feature-flags-api-batch-delete-input-item
source_filename: crm-feature-flags-api-batch-delete-input-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-batch-delete-input-item-schema.json\",\n  \"title\": \"BatchDeleteInputItem\",\n  \"description\": \"Individual item in a batch delete request\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portalId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The unique identifier for the HubSpot portal (account)\",\n      \"example\": 98765432\n    }\n  },\n  \"required\": [\n    \"portalId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-batch-delete-input-item-schema.json
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
