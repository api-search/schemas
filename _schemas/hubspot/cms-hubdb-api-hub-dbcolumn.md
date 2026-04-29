---
description: A column definition in a HubDB table.
layout: schema
name: HubDBColumn
properties_list:
- description: The unique identifier for the column.
  name: id
  type: string
- description: The machine-readable name of the column.
  name: name
  type: string
- description: The human-readable label for the column.
  name: label
  type: string
- description: The data type of the column.
  name: type
  type: string
- description: Available options for SELECT and MULTISELECT columns.
  name: options
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/cms-hubdb-api-hub-dbcolumn-schema.json
slug: cms-hubdb-api-hub-dbcolumn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-hub-dbcolumn-schema.json\",\n  \"title\": \"HubDBColumn\",\n  \"description\": \"A column definition in a HubDB table.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the column.\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The machine-readable name of the column.\",\n      \"example\": \"Example Record\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable label for the column.\",\n      \"example\": \"Example Record\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the column.\",\n      \"enum\": [\n        \"TEXT\",\n        \"NUMBER\"\
  ,\n        \"URL\",\n        \"IMAGE\",\n        \"SELECT\",\n        \"MULTISELECT\",\n        \"BOOLEAN\",\n        \"LOCATION\",\n        \"DATE\",\n        \"DATETIME\",\n        \"CURRENCY\",\n        \"RICHTEXT\",\n        \"FOREIGN_ID\"\n      ],\n      \"example\": \"TEXT\"\n    },\n    \"options\": {\n      \"type\": \"array\",\n      \"description\": \"Available options for SELECT and MULTISELECT columns.\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"example\": [\n        {}\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-hub-dbcolumn-schema.json
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
title: HubDBColumn
---
