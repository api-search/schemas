---
description: Request to create an Excel workbook
layout: schema
name: WorkbookRequest
properties_list:
- description: Workbook filename
  name: name
  type: string
- description: Output format
  name: format
  type: string
- description: Initial sheet names
  name: sheets
  type: array
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-workbook-request-schema.json
slug: apache-poi-workbook-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-workbook-request-schema.json\",\n  \"title\": \"WorkbookRequest\",\n  \"description\": \"Request to create an Excel workbook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Workbook filename\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"XLS\",\n        \"XLSX\"\n      ],\n      \"description\": \"Output format\"\n    },\n    \"sheets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Initial sheet names\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"format\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-workbook-request-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: WorkbookRequest
---
