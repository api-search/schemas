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
schema_file: json-schema/crm-associations-api-batch-association-read-input-schema.json
slug: crm-associations-api-batch-association-read-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-batch-association-read-input-schema.json\",\n  \"title\": \"BatchAssociationReadInput\",\n  \"description\": \"Input for batch reading associations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Reference to a CRM object by ID\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the object\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      },\n      \"description\": \"Source objects to read associations for\",\n      \"example\": [\n        {\n          \"id\": \"500123\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-batch-association-read-input-schema.json
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
