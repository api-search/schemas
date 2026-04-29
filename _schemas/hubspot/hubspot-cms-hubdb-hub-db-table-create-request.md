---
description: Request body for creating or updating a HubDB table.
layout: schema
name: HubDBTableCreateRequest
properties_list:
- description: The machine-readable name of the table.
  name: name
  type: string
- description: The human-readable label for the table.
  name: label
  type: string
- description: ''
  name: columns
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-cms-hubdb-hub-db-table-create-request-schema.json
slug: hubspot-cms-hubdb-hub-db-table-create-request
source_filename: hubspot-cms-hubdb-hub-db-table-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for creating or updating a HubDB table.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The machine-readable name of the table.\",\n      \"example\": \"Example Record\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable label for the table.\",\n      \"example\": \"Example Record\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"name\": \"Example Record\",\n          \"label\": \"Example Record\",\n          \"type\": \"standard\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"label\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n\
  \  },\n  \"required\": [\n    \"name\",\n    \"label\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HubDBTableCreateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-cms-hubdb-hub-db-table-create-request-schema.json
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
title: HubDBTableCreateRequest
---
