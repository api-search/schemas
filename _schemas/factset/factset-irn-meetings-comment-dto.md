---
description: ''
layout: schema
name: CommentDto
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: authorId
  type: string
- description: ''
  name: parentCommentId
  type: string
- description: ''
  name: body
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: attachments
  type: array
- description: ''
  name: subcomments
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-meetings-comment-dto-schema.json
slug: factset-irn-meetings-comment-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommentDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"authorId\": {\n      \"type\": \"string\"\n    },\n    \"parentCommentId\": {\n      \"type\": \"string\"\n    },\n    \"body\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"attachments\": {\n      \"type\": \"array\"\n    },\n    \"subcomments\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-meetings-comment-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CommentDto
---
