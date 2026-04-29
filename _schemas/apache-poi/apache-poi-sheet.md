---
description: Excel worksheet
layout: schema
name: Sheet
properties_list:
- description: Sheet name
  name: name
  type: string
- description: Sheet index (0-based)
  name: index
  type: integer
- description: Number of rows with data
  name: rowCount
  type: integer
- description: Number of columns with data
  name: columnCount
  type: integer
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-sheet-schema.json
slug: apache-poi-sheet
source_filename: apache-poi-sheet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-sheet-schema.json\",\n  \"title\": \"Sheet\",\n  \"description\": \"Excel worksheet\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Sheet name\"\n    },\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"Sheet index (0-based)\"\n    },\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows with data\"\n    },\n    \"columnCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of columns with data\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-sheet-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: Sheet
---
