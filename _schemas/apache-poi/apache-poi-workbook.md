---
description: Excel workbook metadata
layout: schema
name: Workbook
properties_list:
- description: Workbook identifier
  name: id
  type: string
- description: Workbook filename
  name: name
  type: string
- description: Office format (legacy XLS or modern XLSX)
  name: format
  type: string
- description: Number of sheets in the workbook
  name: sheetCount
  type: integer
- description: Creation timestamp
  name: createdAt
  type: string
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-workbook-schema.json
slug: apache-poi-workbook
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-workbook-schema.json\",\n  \"title\": \"Workbook\",\n  \"description\": \"Excel workbook metadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Workbook identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Workbook filename\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"XLS\",\n        \"XLSX\"\n      ],\n      \"description\": \"Office format (legacy XLS or modern XLSX)\"\n    },\n    \"sheetCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of sheets in the workbook\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-workbook-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: Workbook
---
