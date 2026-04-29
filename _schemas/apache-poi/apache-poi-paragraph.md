---
description: Paragraph in a Word document
layout: schema
name: Paragraph
properties_list:
- description: Paragraph index
  name: index
  type: integer
- description: Paragraph text content
  name: text
  type: string
- description: Paragraph style name
  name: style
  type: string
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-paragraph-schema.json
slug: apache-poi-paragraph
source_filename: apache-poi-paragraph-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-paragraph-schema.json\",\n  \"title\": \"Paragraph\",\n  \"description\": \"Paragraph in a Word document\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"Paragraph index\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Paragraph text content\"\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"Paragraph style name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-paragraph-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: Paragraph
---
