---
description: Document conversion result
layout: schema
name: ConversionResult
properties_list:
- description: Converted document identifier
  name: id
  type: string
- description: Output format
  name: format
  type: string
- description: Download URL for the converted document
  name: url
  type: string
- description: File size in bytes
  name: size
  type: integer
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-conversion-result-schema.json
slug: apache-poi-conversion-result
source_filename: apache-poi-conversion-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-conversion-result-schema.json\",\n  \"title\": \"ConversionResult\",\n  \"description\": \"Document conversion result\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Converted document identifier\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Output format\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Download URL for the converted document\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"File size in bytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-conversion-result-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: ConversionResult
---
