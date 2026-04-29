---
description: A comment on a report or expense
layout: schema
name: Comment
properties_list:
- description: The comment text content
  name: comment
  type: string
- description: The user who authored the comment
  name: author
  type: object
- description: When the comment was created
  name: creationDate
  type: string
- description: Whether this is the most recent comment
  name: isLatest
  type: boolean
- description: Whether this is a system-generated audit entry
  name: isAuditLog
  type: boolean
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-comment-schema.json
slug: sap-concur-expense-comment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Comment\",\n  \"type\": \"object\",\n  \"description\": \"A comment on a report or expense\",\n  \"properties\": {\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"The comment text content\"\n    },\n    \"author\": {\n      \"type\": \"object\",\n      \"description\": \"The user who authored the comment\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"description\": \"When the comment was created\"\n    },\n    \"isLatest\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the most recent comment\"\n    },\n    \"isAuditLog\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a system-generated audit entry\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-comment-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: Comment
---
