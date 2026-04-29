---
description: Request body for creating or updating a HubDB table row.
layout: schema
name: HubDBRowCreateRequest
properties_list:
- description: The column values for the row as key-value pairs.
  name: values
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-cms-hubdb-hub-db-row-create-request-schema.json
slug: hubspot-cms-hubdb-hub-db-row-create-request
source_filename: hubspot-cms-hubdb-hub-db-row-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for creating or updating a HubDB table row.\",\n  \"properties\": {\n    \"values\": {\n      \"type\": \"object\",\n      \"description\": \"The column values for the row as key-value pairs.\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HubDBRowCreateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-cms-hubdb-hub-db-row-create-request-schema.json
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
title: HubDBRowCreateRequest
---
