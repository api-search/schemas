---
description: List of sheets in a workbook
layout: schema
name: SheetList
properties_list:
- description: ''
  name: sheets
  type: array
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-sheet-list-schema.json
slug: apache-poi-sheet-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-sheet-list-schema.json\",\n  \"title\": \"SheetList\",\n  \"description\": \"List of sheets in a workbook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sheets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Sheet\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-sheet-list-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: SheetList
---
