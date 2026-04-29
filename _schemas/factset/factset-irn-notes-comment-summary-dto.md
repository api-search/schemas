---
description: ''
layout: schema
name: CommentSummaryDto
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: userId
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: subcomments
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-notes-comment-summary-dto-schema.json
slug: factset-irn-notes-comment-summary-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommentSummaryDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"userId\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"subcomments\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-notes-comment-summary-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CommentSummaryDto
---
