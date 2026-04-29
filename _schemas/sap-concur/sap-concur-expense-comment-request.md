---
description: Request body for creating or updating a comment
layout: schema
name: CommentRequest
properties_list:
- description: The comment text content
  name: comment
  type: string
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-comment-request-schema.json
slug: sap-concur-expense-comment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommentRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating or updating a comment\",\n  \"properties\": {\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"The comment text content\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-comment-request-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: CommentRequest
---
