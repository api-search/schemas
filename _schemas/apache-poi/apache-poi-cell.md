---
description: Individual Excel cell
layout: schema
name: Cell
properties_list:
- description: Cell address (e.g. A1)
  name: address
  type: string
- description: Cell value as string
  name: value
  type: string
- description: Cell type
  name: type
  type: string
- description: Formula if applicable
  name: formula
  type: string
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-cell-schema.json
slug: apache-poi-cell
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-cell-schema.json\",\n  \"title\": \"Cell\",\n  \"description\": \"Individual Excel cell\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Cell address (e.g. A1)\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Cell value as string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"STRING\",\n        \"NUMERIC\",\n        \"BOOLEAN\",\n        \"FORMULA\",\n        \"BLANK\",\n        \"ERROR\"\n      ],\n      \"description\": \"Cell type\"\n    },\n    \"formula\": {\n      \"type\": \"string\",\n      \"description\": \"Formula if applicable\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-cell-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: Cell
---
