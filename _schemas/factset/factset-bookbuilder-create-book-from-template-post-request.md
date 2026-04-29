---
description: It is a request body to allow users to input ticker and template id.
layout: schema
name: createBookFromTemplatePostRequest
properties_list:
- description: ticker
  name: ticker
  type: string
- description: Template ID
  name: template_id
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-bookbuilder-create-book-from-template-post-request-schema.json
slug: factset-bookbuilder-create-book-from-template-post-request
source_filename: factset-bookbuilder-create-book-from-template-post-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"createBookFromTemplatePostRequest\",\n  \"type\": \"object\",\n  \"description\": \"It is a request body to allow users to input ticker and template id.\",\n  \"properties\": {\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"ticker\"\n    },\n    \"template_id\": {\n      \"type\": \"string\",\n      \"description\": \"Template ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-bookbuilder-create-book-from-template-post-request-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: createBookFromTemplatePostRequest
---
