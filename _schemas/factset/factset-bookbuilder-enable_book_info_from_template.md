---
description: Request to enable book information for the client.
layout: schema
name: Enable_Book_Info_From_Template
properties_list:
- description: Request status
  name: status
  type: string
- description: Report Name
  name: bookName
  type: string
- description: Book ID
  name: bookID
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-bookbuilder-enable_book_info_from_template-schema.json
slug: factset-bookbuilder-enable_book_info_from_template
source_filename: factset-bookbuilder-enable_book_info_from_template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Enable_Book_Info_From_Template\",\n  \"type\": \"object\",\n  \"description\": \"Request to enable book information for the client.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Request status\"\n    },\n    \"bookName\": {\n      \"type\": \"string\",\n      \"description\": \"Report Name\"\n    },\n    \"bookID\": {\n      \"type\": \"string\",\n      \"description\": \"Book ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-bookbuilder-enable_book_info_from_template-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Enable_Book_Info_From_Template
---
