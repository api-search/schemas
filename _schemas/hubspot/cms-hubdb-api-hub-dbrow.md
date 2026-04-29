---
description: A row in a HubDB table.
layout: schema
name: HubDBRow
properties_list:
- description: The unique identifier for the row.
  name: id
  type: string
- description: The column values for the row as key-value pairs.
  name: values
  type: object
- description: The date and time the row was created.
  name: createdAt
  type: string
- description: The date and time the row was last updated.
  name: updatedAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/cms-hubdb-api-hub-dbrow-schema.json
slug: cms-hubdb-api-hub-dbrow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-hub-dbrow-schema.json\",\n  \"title\": \"HubDBRow\",\n  \"description\": \"A row in a HubDB table.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the row.\",\n      \"example\": \"500123\"\n    },\n    \"values\": {\n      \"type\": \"object\",\n      \"description\": \"The column values for the row as key-value pairs.\",\n      \"additionalProperties\": true,\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the row was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date-time\",\n      \"description\": \"The date and time the row was last updated.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-hub-dbrow-schema.json
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
title: HubDBRow
---
