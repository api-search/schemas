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
schema_file: json-schema/cms-hubdb-api-hub-dbrow-create-request-schema.json
slug: cms-hubdb-api-hub-dbrow-create-request
source_filename: cms-hubdb-api-hub-dbrow-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-hub-dbrow-create-request-schema.json\",\n  \"title\": \"HubDBRowCreateRequest\",\n  \"description\": \"Request body for creating or updating a HubDB table row.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"values\": {\n      \"type\": \"object\",\n      \"description\": \"The column values for the row as key-value pairs.\",\n      \"additionalProperties\": true,\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-hub-dbrow-create-request-schema.json
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
