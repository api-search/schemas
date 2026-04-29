---
description: Document conversion request
layout: schema
name: ConversionRequest
properties_list:
- description: Source document identifier
  name: sourceId
  type: string
- description: Type of the source document
  name: sourceType
  type: string
- description: Target format (XLSX, DOCX, PPTX, PDF)
  name: targetFormat
  type: string
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-conversion-request-schema.json
slug: apache-poi-conversion-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-conversion-request-schema.json\",\n  \"title\": \"ConversionRequest\",\n  \"description\": \"Document conversion request\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceId\": {\n      \"type\": \"string\",\n      \"description\": \"Source document identifier\"\n    },\n    \"sourceType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"workbook\",\n        \"document\",\n        \"presentation\"\n      ],\n      \"description\": \"Type of the source document\"\n    },\n    \"targetFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Target format (XLSX, DOCX, PPTX, PDF)\"\n    }\n  },\n  \"required\": [\n    \"sourceId\",\n    \"sourceType\",\n    \"targetFormat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-conversion-request-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: ConversionRequest
---
