---
description: List of Excel workbooks
layout: schema
name: WorkbookList
properties_list:
- description: ''
  name: workbooks
  type: array
- description: Total number of workbooks
  name: total
  type: integer
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-workbook-list-schema.json
slug: apache-poi-workbook-list
source_filename: apache-poi-workbook-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-workbook-list-schema.json\",\n  \"title\": \"WorkbookList\",\n  \"description\": \"List of Excel workbooks\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workbooks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Workbook\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of workbooks\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-workbook-list-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: WorkbookList
---
