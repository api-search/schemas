---
description: Request to download book.
layout: schema
name: Enable_Book_Download
properties_list:
- description: Book status
  name: Message
  type: string
- description: URL to book.
  name: url
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-bookbuilder-enable_book_download-schema.json
slug: factset-bookbuilder-enable_book_download
source_filename: factset-bookbuilder-enable_book_download-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Enable_Book_Download\",\n  \"type\": \"object\",\n  \"description\": \"Request to download book.\",\n  \"properties\": {\n    \"Message\": {\n      \"type\": \"string\",\n      \"description\": \"Book status\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to book.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-bookbuilder-enable_book_download-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Enable_Book_Download
---
