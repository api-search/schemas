---
description: Word document
layout: schema
name: Document
properties_list:
- description: Document identifier
  name: id
  type: string
- description: Document filename
  name: name
  type: string
- description: Document format
  name: format
  type: string
- description: ''
  name: paragraphs
  type: array
- description: Estimated page count
  name: pageCount
  type: integer
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-document-schema.json
slug: apache-poi-document
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-document-schema.json\",\n  \"title\": \"Document\",\n  \"description\": \"Word document\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Document identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Document filename\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DOC\",\n        \"DOCX\"\n      ],\n      \"description\": \"Document format\"\n    },\n    \"paragraphs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Paragraph\"\n      }\n    },\n    \"pageCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Estimated page count\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-document-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: Document
---
