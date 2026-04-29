---
description: Associated Error Objects
layout: schema
name: ErrorObject
properties_list:
- description: A unique ID for the occurrence of the error. It is advised to log this code and include it if you contact FactSet support desk.
  name: id
  type: string
- description: a description of the error
  name: title
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-universal-screening-error-object-schema.json
slug: factset-universal-screening-error-object
source_filename: factset-universal-screening-error-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorObject\",\n  \"type\": \"object\",\n  \"description\": \"Associated Error Objects\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique ID for the occurrence of the error. It is advised to log this code and include it if you contact FactSet support desk.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"a description of the error\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-universal-screening-error-object-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ErrorObject
---
