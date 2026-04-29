---
description: The request body allows users to input the name of the book, ticker
layout: schema
name: createBookPostRequest
properties_list:
- description: name of the book
  name: book_name
  type: string
- description: Identifier.
  name: ticker
  type: string
- description: options for pagination
  name: pagination
  type: object
- description: Content sections
  name: content
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-bookbuilder-create-book-post-request-schema.json
slug: factset-bookbuilder-create-book-post-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"createBookPostRequest\",\n  \"type\": \"object\",\n  \"description\": \"The request body allows users to input the name of the book, ticker\",\n  \"properties\": {\n    \"book_name\": {\n      \"type\": \"string\",\n      \"description\": \"name of the book\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier.\"\n    },\n    \"pagination\": {\n      \"type\": \"object\",\n      \"description\": \"options for pagination\"\n    },\n    \"content\": {\n      \"type\": \"array\",\n      \"description\": \"Content sections\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-bookbuilder-create-book-post-request-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: createBookPostRequest
---
