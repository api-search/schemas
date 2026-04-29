---
description: Input payload for batch deleting portal flag states
layout: schema
name: BatchDeleteInput
properties_list:
- description: List of portal IDs to delete flag states for
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-feature-flags-batch-delete-input-schema.json
slug: hubspot-crm-feature-flags-batch-delete-input
source_filename: hubspot-crm-feature-flags-batch-delete-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input payload for batch deleting portal flag states\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"List of portal IDs to delete flag states for\",\n      \"example\": [\n        {\n          \"portalId\": 98765432\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Individual item in a batch delete request\",\n        \"properties\": {\n          \"portalId\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique identifier for the HubSpot portal (account)\",\n            \"format\": \"int64\",\n            \"example\": 98765432\n          }\n        },\n        \"required\": [\n          \"portalId\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchDeleteInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-batch-delete-input-schema.json
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
title: BatchDeleteInput
---
