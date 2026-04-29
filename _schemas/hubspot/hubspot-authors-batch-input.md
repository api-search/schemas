---
description: Input for batch update operations
layout: schema
name: BatchInput
properties_list:
- description: Array of items to process
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-authors-batch-input-schema.json
slug: hubspot-authors-batch-input
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input for batch update operations\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of items to process\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"properties\": {}\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Single item in a batch update operation\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the author to update\",\n            \"example\": \"500123\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"Input data for creating or updating a blog author\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Full display name of the author\",\n                \"example\"\
  : \"Example Record\"\n              },\n              \"slug\": {\n                \"type\": \"string\",\n                \"description\": \"URL-friendly identifier for the author\",\n                \"example\": \"example-value\"\n              },\n              \"email\": {\n                \"type\": \"string\",\n                \"description\": \"Author's email address\",\n                \"format\": \"email\",\n                \"example\": \"jsmith@example.com\"\n              },\n              \"bio\": {\n                \"type\": \"string\",\n                \"description\": \"Author biography or description\",\n                \"example\": \"example-value\"\n              },\n              \"website\": {\n                \"type\": \"string\",\n                \"description\": \"Author's personal website URL\",\n                \"format\": \"uri\",\n                \"example\": \"https://app.hubspot.com/contacts/12345\"\n              },\n              \"twitter\": {\n          \
  \      \"type\": \"string\",\n                \"description\": \"Author's Twitter/X handle\",\n                \"example\": \"example-value\"\n              },\n              \"facebook\": {\n                \"type\": \"string\",\n                \"description\": \"Author's Facebook profile URL\",\n                \"example\": \"example-value\"\n              },\n              \"linkedin\": {\n                \"type\": \"string\",\n                \"description\": \"Author's LinkedIn profile URL\",\n                \"example\": \"https://app.hubspot.com/contacts/12345\"\n              },\n              \"avatar\": {\n                \"type\": \"string\",\n                \"description\": \"URL to the author's avatar image\",\n                \"format\": \"uri\",\n                \"example\": \"https://app.hubspot.com/contacts/12345\"\n              }\n            },\n            \"required\": [\n              \"name\"\n            ]\n          }\n        },\n        \"required\": [\n \
  \         \"id\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-authors-batch-input-schema.json
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
title: BatchInput
---
