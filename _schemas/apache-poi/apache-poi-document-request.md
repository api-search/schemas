---
description: Request to create a Word document
layout: schema
name: DocumentRequest
properties_list:
- description: Document filename
  name: name
  type: string
- description: Document format
  name: format
  type: string
- description: Initial text content
  name: content
  type: string
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-document-request-schema.json
slug: apache-poi-document-request
source_filename: apache-poi-document-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-document-request-schema.json\",\n  \"title\": \"DocumentRequest\",\n  \"description\": \"Request to create a Word document\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Document filename\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DOC\",\n        \"DOCX\"\n      ],\n      \"description\": \"Document format\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Initial text content\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"format\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-document-request-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: DocumentRequest
---
