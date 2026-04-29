---
description: Input for batch create operations
layout: schema
name: BatchCreateInput
properties_list:
- description: Array of authors to create
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/authors-api-batch-create-input-schema.json
slug: authors-api-batch-create-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-batch-create-input-schema.json\",\n  \"title\": \"BatchCreateInput\",\n  \"description\": \"Input for batch create operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Input data for creating or updating a blog author\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Full display name of the author\",\n            \"example\": \"Example Record\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"URL-friendly identifier for the author\",\n            \"example\": \"example-value\"\n          },\n          \"email\": {\n            \"type\": \"string\"\
  ,\n            \"format\": \"email\",\n            \"description\": \"Author's email address\",\n            \"example\": \"jsmith@example.com\"\n          },\n          \"bio\": {\n            \"type\": \"string\",\n            \"description\": \"Author biography or description\",\n            \"example\": \"example-value\"\n          },\n          \"website\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"Author's personal website URL\",\n            \"example\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"twitter\": {\n            \"type\": \"string\",\n            \"description\": \"Author's Twitter/X handle\",\n            \"example\": \"example-value\"\n          },\n          \"facebook\": {\n            \"type\": \"string\",\n            \"description\": \"Author's Facebook profile URL\",\n            \"example\": \"example-value\"\n          },\n          \"linkedin\": {\n            \"type\": \"\
  string\",\n            \"description\": \"Author's LinkedIn profile URL\",\n            \"example\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"avatar\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"URL to the author's avatar image\",\n            \"example\": \"https://app.hubspot.com/contacts/12345\"\n          }\n        },\n        \"required\": [\n          \"name\"\n        ]\n      },\n      \"description\": \"Array of authors to create\",\n      \"example\": [\n        {\n          \"name\": \"Example Record\",\n          \"slug\": \"example-value\",\n          \"email\": \"jsmith@example.com\",\n          \"bio\": \"example-value\",\n          \"website\": \"https://app.hubspot.com/contacts/12345\",\n          \"twitter\": \"example-value\",\n          \"facebook\": \"example-value\",\n          \"linkedin\": \"https://app.hubspot.com/contacts/12345\",\n          \"avatar\": \"https://app.hubspot.com/contacts/12345\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-batch-create-input-schema.json
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
title: BatchCreateInput
---
