---
description: ''
layout: schema
name: CreateCommentDto
properties_list:
- description: ''
  name: authorId
  type: string
- description: ''
  name: parentCommentId
  type: string
- description: ''
  name: body
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-notes-create-comment-dto-schema.json
slug: factset-irn-notes-create-comment-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateCommentDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorId\": {\n      \"type\": \"string\"\n    },\n    \"parentCommentId\": {\n      \"type\": \"string\"\n    },\n    \"body\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-notes-create-comment-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CreateCommentDto
---
