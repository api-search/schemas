---
description: Cell data from an Excel sheet
layout: schema
name: CellData
properties_list:
- description: ''
  name: rows
  type: array
- description: Cell range returned
  name: range
  type: string
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-cell-data-schema.json
slug: apache-poi-cell-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-cell-data-schema.json\",\n  \"title\": \"CellData\",\n  \"description\": \"Cell data from an Excel sheet\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rows\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"$ref\": \"#/components/schemas/Cell\"\n        }\n      }\n    },\n    \"range\": {\n      \"type\": \"string\",\n      \"description\": \"Cell range returned\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-cell-data-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: CellData
---
