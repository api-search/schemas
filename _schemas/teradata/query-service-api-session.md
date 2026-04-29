---
description: A query session.
layout: schema
name: Session
properties_list:
- description: Unique session identifier.
  name: sessionId
  type: string
- description: Connected system name.
  name: system
  type: string
- description: Default database.
  name: database
  type: string
- description: Session status.
  name: status
  type: string
- description: Session creation time.
  name: createdAt
  type: string
provider_name: Teradata
provider_slug: teradata
schema_file: json-schema/query-service-api-session-schema.json
slug: query-service-api-session
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/query-service-api-session-schema.json\",\n  \"title\": \"Session\",\n  \"description\": \"A query session.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": { \"type\": \"string\", \"description\": \"Unique session identifier.\" },\n    \"system\": { \"type\": \"string\", \"description\": \"Connected system name.\" },\n    \"database\": { \"type\": \"string\", \"description\": \"Default database.\" },\n    \"status\": { \"type\": \"string\", \"description\": \"Session status.\", \"enum\": [\"active\", \"idle\", \"closed\"] },\n    \"createdAt\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Session creation time.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/query-service-api-session-schema.json
tags:
- Analytics
- Cloud
- Data Management
- Data Warehousing
- Database
- Enterprise
- Machine Learning
- SQL
title: Session
---
