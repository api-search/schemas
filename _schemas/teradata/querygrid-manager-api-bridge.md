---
description: A bridge connecting two systems.
layout: schema
name: Bridge
properties_list:
- description: Unique bridge identifier.
  name: id
  type: string
- description: Bridge name.
  name: name
  type: string
- description: Source system identifier.
  name: sourceSystemId
  type: string
- description: Target system identifier.
  name: targetSystemId
  type: string
- description: Bridge status.
  name: status
  type: string
provider_name: Teradata
provider_slug: teradata
schema_file: json-schema/querygrid-manager-api-bridge-schema.json
slug: querygrid-manager-api-bridge
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-bridge-schema.json\",\n  \"title\": \"Bridge\",\n  \"description\": \"A bridge connecting two systems.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique bridge identifier.\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Bridge name.\" },\n    \"sourceSystemId\": { \"type\": \"string\", \"description\": \"Source system identifier.\" },\n    \"targetSystemId\": { \"type\": \"string\", \"description\": \"Target system identifier.\" },\n    \"status\": { \"type\": \"string\", \"description\": \"Bridge status.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-bridge-schema.json
tags:
- Analytics
- Cloud
- Data Management
- Data Warehousing
- Database
- Enterprise
- Machine Learning
- SQL
title: Bridge
---
