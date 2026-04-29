---
description: A HubDB table.
layout: schema
name: HubDBTable
properties_list:
- description: The unique identifier for the table.
  name: id
  type: string
- description: The machine-readable name of the table.
  name: name
  type: string
- description: The human-readable label for the table.
  name: label
  type: string
- description: The column definitions for the table.
  name: columns
  type: array
- description: Whether the table has been published.
  name: published
  type: boolean
- description: The number of rows in the published table.
  name: rowCount
  type: integer
- description: The date and time the table was created.
  name: createdAt
  type: string
- description: The date and time the table was last updated.
  name: updatedAt
  type: string
- description: The date and time the table was last published.
  name: publishedAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/cms-hubdb-api-hub-dbtable-schema.json
slug: cms-hubdb-api-hub-dbtable
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-hub-dbtable-schema.json\",\n  \"title\": \"HubDBTable\",\n  \"description\": \"A HubDB table.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the table.\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The machine-readable name of the table.\",\n      \"example\": \"Example Record\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable label for the table.\",\n      \"example\": \"Example Record\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"The column definitions for the table.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\"\
  : \"A column definition in a HubDB table.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the column.\",\n            \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The machine-readable name of the column.\",\n            \"example\": \"Example Record\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"description\": \"The human-readable label for the column.\",\n            \"example\": \"Example Record\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The data type of the column.\",\n            \"enum\": [\n              \"TEXT\",\n              \"NUMBER\",\n              \"URL\",\n              \"IMAGE\",\n              \"SELECT\",\n              \"MULTISELECT\",\n              \"BOOLEAN\",\n              \"LOCATION\"\
  ,\n              \"DATE\",\n              \"DATETIME\",\n              \"CURRENCY\",\n              \"RICHTEXT\",\n              \"FOREIGN_ID\"\n            ],\n            \"example\": \"TEXT\"\n          },\n          \"options\": {\n            \"type\": \"array\",\n            \"description\": \"Available options for SELECT and MULTISELECT columns.\",\n            \"items\": {\n              \"type\": \"object\"\n            },\n            \"example\": [\n              {}\n            ]\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"name\": \"Example Record\",\n          \"label\": \"Example Record\",\n          \"type\": \"TEXT\",\n          \"options\": [\n            {}\n          ]\n        }\n      ]\n    },\n    \"published\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the table has been published.\",\n      \"example\": true\n    },\n    \"rowCount\": {\n      \"type\": \"integer\",\n   \
  \   \"description\": \"The number of rows in the published table.\",\n      \"example\": 10\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the table was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the table was last updated.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"publishedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the table was last published.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-hubdb-api-hub-dbtable-schema.json
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
title: HubDBTable
---
