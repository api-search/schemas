---
description: Input for batch reading associations
layout: schema
name: BatchAssociationReadInput
properties_list:
- description: Source objects to read associations for
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-associations-batch-association-read-input-schema.json
slug: hubspot-crm-associations-batch-association-read-input
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input for batch reading associations\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Source objects to read associations for\",\n      \"example\": [\n        {\n          \"id\": \"500123\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Reference to a CRM object by ID\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the object\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchAssociationReadInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-batch-association-read-input-schema.json
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
title: BatchAssociationReadInput
---
