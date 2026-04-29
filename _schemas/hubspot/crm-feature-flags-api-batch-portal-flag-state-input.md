---
description: Input payload for batch creating or updating portal flag states
layout: schema
name: BatchPortalFlagStateInput
properties_list:
- description: List of portal flag state inputs
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-feature-flags-api-batch-portal-flag-state-input-schema.json
slug: crm-feature-flags-api-batch-portal-flag-state-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-batch-portal-flag-state-input-schema.json\",\n  \"title\": \"BatchPortalFlagStateInput\",\n  \"description\": \"Input payload for batch creating or updating portal flag states\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"List of portal flag state inputs\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Individual item in a batch upsert request\",\n        \"required\": [\n          \"portalId\",\n          \"flagState\"\n        ],\n        \"properties\": {\n          \"portalId\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"The unique identifier for the HubSpot portal (account)\",\n            \"example\": 98765432\n \
  \         },\n          \"flagState\": {\n            \"$ref\": \"#/components/schemas/FlagState\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"portalId\": 98765432,\n          \"flagState\": {}\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-batch-portal-flag-state-input-schema.json
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
title: BatchPortalFlagStateInput
---
